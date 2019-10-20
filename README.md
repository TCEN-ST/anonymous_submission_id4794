# anonymous_submission_id4794

## Results for extended librispeech ST dataset
|  setting | test (BLEU) |
| --- | --- |
| Vanilla* | 15.71 |
| +enc pretrain* | 16.30 |
| +enc dec pretrain* | 16.68 |
| Our method | 17.05 |

*The copy the number of baseline settings from <https://github.com/espnet/espnet/blob/master/egs/libri_trans/st1/RESULTS>. We train our model following the same data preprocessing pipeline.

## Results for Transformer architecture on tst2013 (character decoder)
We implement the Transformer backboned model following the paper 
>Speech-Transformer: A No-Recurrence Sequence-to-Sequence Model for Speech Recognition <
We use the big model setting (12Enc6Dec-wide) for both ASR and ST model. For MT model, we use the same encoder-decoder setting with ASR model but replace the conv layer to word embedding.

|  setting | tst2013 (BLEU) |
| --- | --- |
| Vanilla | - |
| +enc pretrain | 13.41 |
| +enc dec pretrain | 14.46 |
| many-to-many + pretrain | 14.98 |
| Our method (Transformer) | 17.11 |

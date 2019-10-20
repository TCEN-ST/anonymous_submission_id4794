# anonymous_submission_id4794

## Results for extended librispeech ST dataset
|  setting | test (BLEU) |
| --- | --- |
| Vanilla* | 15.71 |
| +enc pretrain* | 16.30 |
| +enc dec pretrain* | 16.68 |
| Our method | 17.05 |
* The copy the number of baseline settings from <https://github.com/espnet/espnet/blob/master/egs/libri_trans/st1/RESULTS>. We train our model following the same data preprocessing pipeline and using the same data.

## Results for Transformer architecture on tst2013 (character decoder)
|  setting | tst2013 (BLEU) |
| --- | --- |
| Vanilla | - |
| +enc pretrain | 13.41 |
| +enc dec pretrain | 14.46 |
| many-to-many + pretrain | 14.98 |
| Our method (Transformer) | 17.11 |

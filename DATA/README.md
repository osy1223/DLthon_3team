# Data Directory Tree & Comments

```
DATA
├── test
│   └── test.csv
└── train
    ├── casual
    │   └── sns_casual.csv = band + facebook + nateon + instagram + kakao[1-4]
    ├── non_casual
    │   ├── archived
    │   │   ├── back_translated_bullying.csv
    │   │   ├── back_translated_bullying_2.csv
    │   │   ├── back_translated_extortion.csv
    │   │   ├── back_translated_extortion_2.csv
    │   │   ├── back_translated_threatening.csv
    │   │   ├── back_translated_threatening_2.csv
    │   │   ├── back_translated_threatening_3.csv
    │   │   └── back_translated_workplace.csv
    │   ├── back_translated_non_casual.csv <= all_data.csv
    │   ├── gpt_augmented_non_casual.csv
    │   ├── plain_non_casual.csv
    │   └── spell_checked_non_casual.csv
    ├── Final_Train.csv
    ├── plain_result.csv <= casual + non_casual, 즉시 적용 가능
    ├── result_kakao.csv <= casual + non_casual, 즉시 적용 가능
    └── spell_result.csv <= casual + non_casual, 즉시 적용 가능
    ├── README.md
```

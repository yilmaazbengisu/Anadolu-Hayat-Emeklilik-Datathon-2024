# Customer Life Insurance Product Recommendation

This repository contains data and machine learning model for a project aimed at recommending life insurance products to customers based on various attributes and metrics. This classification problem is both imbalanced and multiclass.

## Dataset Description

The dataset contains information about customers, their demographics, and their interactions with the company's products. Below is a detailed description of the dataset:

### Features

- **MUSTERI_ID**: Unique ID for each customer.
- **LABEL**: Type of life insurance product purchased by the customer.
- **FLAG**: Month to which the data belongs.
- **PP_CINSIYET**: Gender of the policyholder (1: Male, 2: Female).
- **PP_YAS**: Age of the policyholder (in months).
- **PP_MESLEK**: Occupation of the policyholder.
- **PP_MUSTERI_SEGMENTI**: Customer segment of the policyholder:
  - 101: A segment
  - 102: B segment
  - 103: C segment
  - 104: D segment
  - 105: E segment
  - 106: F segment
- **PP_UYRUK**: Nationality of the policyholder:
  - 1: Turkish Citizen
  - 2: Blue Card
  - 3: Foreign National
- **IL**: License plate code of the city where the policyholder lives (0 = Abroad).
- **SORU_YATIRIM_KARAKTERI_CVP**: Investment character based on survey responses.
- **SORU_YATIRIM_KARAKTERI_RG**: Time elapsed since the investment character survey response (in months).
- **SORU_MEDENI_HAL_CVP**: Marital status based on survey responses.
- **SORU_MEDENI_HAL_RG**: Time elapsed since the marital status survey response (in months).
- **SORU_EGITIM_CVP**: Education level based on survey responses.
- **SORU_EGITIM_RG**: Time elapsed since the education level survey response (in months).
- **SORU_GELIR_CVP**: Income level based on survey responses.
- **SORU_GELIR_RG**: Time elapsed since the income level survey response (in months).
- **SORU_COCUK_SAYISI_CVP**: Number of children based on survey responses.
- **SORU_COCUK_SAYISI_RG**: Time elapsed since the number of children survey response (in months).
- **BES_AYRILMA_TALEP_ADET**: Number of requests to withdraw from the BES account.
- **ODEMEME_TALEP_ADET**: Number of non-payment instructions given in the last year.
- **HAYAT_AYRILMA_TALEP_ADET**: Number of requests to withdraw from the life insurance.
- **BILGI_TALEP_ADET**: Number of information requests about the policy.
- **VADE_TUTAR_0 - VADE_TUTAR_11**: Total installment amounts for the products owned in the last 12 months.
- **ODEME_TUTAR_0 - ODEME_TUTAR_11**: Payment amounts for the products owned in the last 12 months.
- **SON_AY_KATKI_MIKTARI**: Total additional contribution payments made in the last month (in TL).
- **SON_AY_KATKI_ADET**: Number of additional contribution payments made in the last month.
- **SON_CEYREK_KATKI_MIKTARI**: Total additional contribution payments made in the last quarter (in TL).
- **SON_CEYREK_KATKI_ADET**: Number of additional contribution payments made in the last quarter.
- **SON_SENE_KATKI_MIKTARI**: Total additional contribution payments made in the last year (in TL).
- **SON_SENE_KATKI_ADET**: Number of additional contribution payments made in the last year.
- **ANAPARA**: Total amount of principal invested (in TL).
- **GETIRI**: Total return on the invested principal (in TL).
- **BU1 - BU24**: Ownership status of BES products 1-24 (details provided in a separate document).
- **HU1 - HU19**: Ownership status of life insurance products 1-19 (details provided in a separate document).
- **AKTIF_ILK_POLICE_RG**: Time elapsed since the oldest active policy (in months).

### Custom Metric Coefficients

| Product | Coefficient |
|---------|-------------|
| HU06    | 0.0385      |
| HU07    | 0.0328      |
| HU11    | 0.2791      |
| HU12    | 0.1812      |
| HU14    | 0.0113      |
| HU15    | 0.2952      |
| HU19    | 0.1614      |
| UA      | 0.0001      |



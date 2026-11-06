# Rōz Risk Check

An open-source breast cancer risk questionnaire in Urdu and English, based on the Tyrer-Cuzick (IBIS) model, which we are calibrating for Pakistani women.

Rōz is built by Kitch AI in Lahore, Pakistan.

## Why this exists

Breast cancer is the most common cancer in Pakistan, and most women are diagnosed late. There is no organised screening programme and very few mammography machines, so doctors have to decide who to scan first. The risk models used for that decision elsewhere, such as Gail and Tyrer-Cuzick, were built on Western data and have never been calibrated for Pakistani women.

The Rōz Risk Check gives a woman a private estimate of her lifetime risk on her phone, in her own language, with a clear next step if her risk is high. It also gives her doctor the history that would otherwise take half a consultation to collect.

## What is in this repository

This repository holds the open-source parts of the Risk Check:

- The questionnaire, in Urdu and English, using family terms women here use (Ammi, Nani, Khala)
- The scoring logic that turns answers into a Tyrer-Cuzick-based lifetime risk estimate
- The calibration code and methods we use to re-estimate risk factors and baseline risk from Pakistani data
- The calibrated calculator, once the calibration study is complete

Hosted services, data storage and integrations with hospital or clinic systems are not part of this repository.

## Status

The Risk Check is live as a web questionnaire and around 500 women have used it. Its outputs have been checked against the US National Cancer Institute's Breast Cancer Risk Assessment Tool. We are now moving the questionnaire and scoring logic into this repository.

| Stage | Status |
| --- | --- |
| Questionnaire (Urdu and English) | Live, moving into this repository |
| Tyrer-Cuzick scoring logic | Being rebuilt here |
| Consent and de-identification flow | Planned |
| Calibration for Pakistani women | Study designed, awaiting funding and ethics approval |
| Free calibrated calculator | Planned release after calibration |

## Important

The Rōz Risk Check is a screening aid, not a diagnosis. It does not replace a clinical breast examination, mammography or medical advice. The current version still uses Western reference data, so its estimates for Pakistani women have not yet been validated.

## Contributing

Issues and pull requests are welcome, especially from clinicians, epidemiologists and Urdu speakers. Please do not include any personal or health data in issues or commits.

## Licence

Released under the [MIT Licence](LICENSE).

## Contact

Mehr-un-Nisa Kitchlew and Shehreyar Kitchlew, Kitch AI, Lahore

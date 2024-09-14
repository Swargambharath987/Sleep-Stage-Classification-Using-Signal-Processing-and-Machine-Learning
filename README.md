# Sleep Stage Classification Using Signal Processing and Machine Learning

## Abstract
Sleep plays a pivotal role in determining well-being and quality of life. Difficulties related to sleep affect both mental and physical health. Therefore, diagnosing sleep disorders must be comprehensive. Proper sleep stage classification is essential for the efficient diagnosis of sleep-related disorders. This project focuses on employing signal processing techniques and various machine learning algorithms to classify individuals’ sleep stages.

For this study, we used the Wisconsin Sleep Cohort (WSC) dataset from the National Sleep Research Resource (NSRR). EEG, EOG, and EMG channels (C3_M2, O1_M2, E1, E2, chin, and cchin_l) with sampling frequencies of 100Hz and 200Hz were extracted from polysomnogram data, as these channels provide valuable insights into sleeping patterns.

The sleep stages were classified using bi-orthogonal wavelet filter banks. Signals were decomposed using five-level wavelet decomposition, yielding six sub-bands. The data were then fed into various supervised machine learning classifiers. A combination of channels was used, and their classification performance was analyzed. The highest classification accuracy of 84.2% was achieved using EEG, EOG, and EMG channels combined, sampled at 100Hz, with an Ensemble Bagged Trees (EBT) classifier and 10-fold cross-validation. The results indicated that combining signals improved classification accuracy.

The developed model can be utilized to evaluate sleep quality and aid in diagnosing sleep disorders based on sleep stage classification.

## Methodology
1. **Dataset**: Wisconsin Sleep Cohort (WSC) from NSRR
2. **Channels Used**: EEG, EOG, EMG (C3_M2, O1_M2, E1, E2, chin)
3. **Signal Processing**: Five-level wavelet decomposition
4. **Machine Learning Models**: Supervised learning algorithms including Ensemble Bagged Trees (EBT)
5. **Evaluation**: 10-fold cross-validation

## Experimentation and Challenges

### Extensive ML Algorithm Testing
We experimented with various machine learning algorithms in MATLAB, which sometimes required overnight runs due to the computational complexity of the models.

### Multiple Signal Frequencies & Channels
Our analysis involved testing different signal frequencies (100Hz, 200Hz) and a variety of channels (EEG, EOG, EMG), making the process highly iterative and experimental.

### Data Access
Access to the Wisconsin Sleep Cohort dataset was granted only after our research proposal was approved by the National Sleep Research Resource (NSRR).

### Data Understanding
Interpreting and cleaning the polysomnography data posed a significant challenge due to its complexity and volume.




## Conclusion
Sleep is a crucial factor for overall health and well-being, and accurate diagnosis of sleep disorders is vital. Traditionally, detecting sleep disorders from sleep data manually is time-consuming and prone to errors, making it challenging for doctors. In this study, we presented a simple yet effective machine learning sleep stage classification system using EMG, EEG, and EOG signals.

We used the WSC dataset and pre-processed the data, applied wavelet decomposition, and performed feature extraction. The data were then classified using supervised machine learning techniques into five sleep stages: N1, N2, N3, REM, and wake. We processed the entire dataset consisting of 1123 subjects and 2570 recordings. 

Our proposed method achieved a maximum classification accuracy of 84.2% and a Cohen’s kappa coefficient of 0.7463±0.0005 using five channels (C3_M2, O1_M2, E1, E2, chin) at a 100 Hz sampling frequency, utilizing the Ensemble Bagged Trees classifier with 10-fold cross-validation. These results show that computer-aided techniques can significantly reduce the workload of medical practitioners. Our method is simple, robust, and achieves good results. 

Future research may focus on developing even simpler and more accurate methods for sleep stage classification.

## Results
- **Accuracy**: 84.2%
- **Cohen's Kappa Coefficient**: 0.7463±0.0005
- **Best Classifier**: Ensemble Bagged Trees (EBT)
- **Channels Used**: C3_M2, O1_M2, E1, E2, chin (100 Hz)

## Future Work
Further improvements can be made to this model by exploring more advanced signal processing techniques and novel machine learning approaches. This project can be a foundation for researchers looking to achieve higher classification accuracy and more effective sleep disorder diagnostics.

## References
- National Sleep Research Resource (NSRR) - https://sleepdata.org/
- Wisconsin Sleep Cohort (WSC) Dataset  - https://sleepdata.org/datasets/wsc

---


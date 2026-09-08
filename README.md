# GAN-for-Physics-Simulator

Реализовал и сравнил четыре генеративные моделина табличных данных (10 признаков Хилласа,19k объектов, UCI MAGIC): conditional WGAN, conditional VAE,диффузионную модель (DDPM, v-prediction + Min-SNRweighting) и нормализующий поток RealNVP. Качествогенерации оценивал внешним классификатором (gradient boosting, ROC-AUC «реальное vsсгенерированное»).Лучший результат у RealNVP: ROC-AUC 0.572 против 0.692 у WGAN и 0.651 у диффузии; улучшение достигнуто за счётувеличения числа coupling-слоёв, шириныподсетей и LR-расписания.

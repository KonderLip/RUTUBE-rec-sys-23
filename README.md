# RUTUBE-rec-sys-23
Создание рекомендательной системы видео для пользователей видеохостинга RUTUBE

* [make_train_data](make_train_data.ipynb) - сохраняем историю просмотров другом формате, для обучения нейросети
* [train_roberta](train_roberta.ipynb) - обучаем Roberta, mrr@10 на следующее видео 0.2049
* [nn+als+cb](nn+als+cb.ipynb) - обучения CosineRecommender и ALS для созданиях кандидатов, затем CatBoostRanker для отбора 10 лучших. map@10 для старых пользователей 0.4
В конце ноутбука инференс, средняя скорость 18 в секунду
* [predict_new_users](predict_new_users.ipynb) - делаем рекомендации для новых пользователей

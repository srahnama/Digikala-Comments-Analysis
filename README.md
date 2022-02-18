# Digikala Comments Analysis with RNN - LSTM
### Predicting whether a comment left in [Digikala](https://www.digikala.com/) without any idea about the recommendation, is recommending a product or not.

- The project overview
    - Data Preprocessing
        - Cleaning
        - Converting
        - Checking null
        - Analyzing
        - Normalizing
    - Modeling
        - Tokenizing
        - Vectorizing
        - Creating model
        - Training model
        - Evaluating model

![alt text](https://raw.githubusercontent.com/srahnama/Digikala-Comments-Analysis/main/wordcloud.png)

### Example results

```Python
model.predict(vectorize_layer(['خیلی بد بود']))
array([[0.23936771]], dtype=float32)

model.predict(vectorize_layer(['افتضاح بود']))
array([[0.04372201]], dtype=float32)

model.predict(vectorize_layer(['عالی بود']))
array([[0.99864143]], dtype=float32)

model.predict(vectorize_layer(['من از این محصول رضایت دارم']))
array([[0.99523926]], dtype=float32)

model.predict(vectorize_layer(['با این قیمت ارزش خرید ندارد']))
array([[0.11104872]], dtype=float32)

model.predict(vectorize_layer(['با این قیمت ارزش خرید دارد']))
array([[0.9712803]], dtype=float32)
```

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

by : [Shahab Rahnama](http://srahnama.ir/)
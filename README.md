#Simple Feature columns for ball strike
```
for prediction, element, hit in zip(predictions[:20], list(res.as_numpy_iterator())[:20], list(test_ds)[0][1][:20]):
  prediction = tf.sigmoid(prediction).numpy()
  print("Predicted: {:.2}".format(prediction[0]),
        element,
        " | Actual outcome: ",
        ("Hit" if bool(hit) else "Strike"))

```

![alt text](https://github.com/HsingYo/Exercise_Tensorflow/blob/master/predict.jpg)

# DeepLearningAI


## 1. Introduction to TensorFlow for Artificial Intelligence, Machine Learning, and Deep Learning
- https://www.coursera.org/learn/introduction-tensorflow?specialization=tensorflow-in-practice
- done, https://coursera.org/share/a4b22430b8431fd2a819361efb2f6011
- 練習實做很接地氣, 測驗發現之前的注意沒有到位的地方,評分的實做有變化, 體會課程安排者的用心。整個online環境優質, 免去配置可能的意外, 有利課程順利進行。
 

### Week3, 2022/3/13, 實做遇到障礙, 困知勉行, 這階段已知其然, 不完全知其所以然,還是很快樂
- reshape and normalize
  - 還不確定為何要加一個維度, 雖然按要求加上, 如同 expected 的值
  - 數值是浮點或是整數可以從錯誤信息修正
- callback
  - 本身要有python的基本參數,調用時不必給的那個
  - 達到預期目標時停止學習, 要注意檢查的值的格式和口語的講法

## 2. Convolutional Neural Networks in TensorFlow
- https://www.coursera.org/learn/convolutional-neural-networks-tensorflow?specialization=tensorflow-in-practice
### Week1, 2022/3/20, 基本的 Python 處理 file, size, Random 
- 要排除不良的樣本, 檔案大小為0
- 要能夠按比例隨機區分到  training and testing, 
  - 另有主題在 training and testing 之外還有 validation 
  - https://developers.google.com/machine-learning/crash-course/validation/video-lecture
- 上述按比例, 先用隨機值來區分, 和預期的並不完成相同, 因為是隨機數, 大比例是對, 但不會保證額定值百分百一樣。先看提交是否可以通過。
- 訓練要運行多分鐘, 單次 epoch 100 杪, 這也是日後要注意的要點。
  - AlphaGo Zero 訓練 40 days X 4 TPU
    - https://en.wikipedia.org/wiki/AlphaGo_Zero#:~:text=Oren%20Etzioni%20of%20the%20Allen,days%2C%20on%20four%20TPUs%22.
- 理論上, 應該設置 callbakcs, https://towardsdatascience.com/neural-network-with-tensorflow-how-to-stop-training-using-callback-5c8d575c18a9, 但在給的模板裡,這部份沒有列出, 不確定在直接給定的 15 epoch 是否能達到 a training accuracy of at least 95% and a validation accuracy of at least 80%.
  - 95s 84ms/step - loss: 0.2808 - accuracy: 0.9053 - val_loss: 0.5656 - val_accuracy: 0.8032 
  - https://youtu.be/wjqaz6m42wU NIPS 2016 tutorial: "Nuts and bolts of building AI applications using Deep Learning" by Andrew Ng
- to fix 90% 10% 區分 training testing
- to add callback to ensure, hopefully, reach min requirement accuracy of at least 95%
- 調了幾種都沒能在 epoch 30次內達到 accuracy 95%, 都在 90和91%之間起落。
- 遇到GPU不給用, 看了說明, 升級為colab Pro用戶。
- 多次嘗試, 終於找到解法。在這過程, 感受到這方面的調試模式。
### Week2, 2022/3/21, 課程教了新的訓練方式, 測驗使用上週實做為基礎
- 訓練越來越費時, 考慮升級Colab PRO 至 PRO+

## 3. Natural Language Processing in TensorFlow
- https://www.coursera.org/learn/natural-language-processing-tensorflow?specialization=tensorflow-in-practice

## 4. Sequences, Time Series and Prediction
- https://www.coursera.org/learn/tensorflow-sequences-time-series-and-prediction?specialization=tensorflow-in-practice


## DeepLearning.AI TensorFlow Developer
- https://www.coursera.org/professional-certificates/tensorflow-in-practice

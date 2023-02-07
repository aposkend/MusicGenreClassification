# MusicGenreClassification

介紹：https://drive.google.com/file/d/1pfpDK3ToswrLq0RI65SopvH7DNHIN4cv/view?usp=sharing

這是一個基於CNN所做的曲風辨識服務，我們對input data進行頻率採樣，並提取mfcc特徵製作成圖片，再使用Resnet50v2進行訓練得到模型，最後使用Gradio套件做出網站式的服務

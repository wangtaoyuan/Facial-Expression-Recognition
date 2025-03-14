|分支示意|实验记录|作者原文|
|----|----|----|
|[:deciduous_tree:](#分支示意 "branch")|[:pencil2:](#实验记录 "wty的实验记录")| [:book:](#作者原文 "原作者的实验说明")|  
  
[表情数据库fer2013地址](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data)

## 分支示意
```mermaid
graph LR
master[master 当前本版] --- version{version}
    version --> |作者原版| D[original]
    version --> |更改版本| E[v 1.0]
```

##  实验记录
2019.06.27用自己的电脑训练了一下模型  
方法：  
        1. 在main.py中更改mode，把“demo”改成“train”；  
        2. 在data文件夹下copy入下载的kaggle数据包文件夹——fer2013  
        3. 运行main.py。  
耗时：7h6min  
电脑配置：  
        win10（64）  
        cpu：corei5 4210M  
        Gpu：Nvidia GeForce840M  
        运存：8GB  

-----------------------
## 作者原文
-------------------------------------------------------------------------------

![amazing](./amazingkelly.jpeg)

Opensource deep learning framework [TensorFlow](https://www.tensorflow.org) is used in **Facial Expression Recognition(FER)**. 
The trained models achieved 65% accuracy in fer2013. If you like this, please give me a star.

#### Dependencies

FER requires:
- Python (>= 3.3)
- TensorFlow (>= 1.1.0) [Installation](https://www.tensorflow.org/install/)
- OpenCV (python3-version) [Installation](http://docs.opencv.org/master/da/df6/tutorial_py_table_of_contents_setup.html)

Only tested in Ubuntu and macOS Sierra. Other platforms are not sure work well. When problems meet, open an issue, I'll do my best to solve that.

#### Usage
###### demo
To run the demo, just type:
​```shell
python3 main.py
```
Then the program will creat a window to display the scene capture by webcamera. You need press <kbd>SPACE</kbd> key to capture face in current frame and recognize the facial expression.

If you just want to run this demo instead of training the model from scaratch, the following content can be skipped.

###### train models
If you want to train a model from scaratch by yourself, download the fer2013 datasets in [kaggle(91.97MB)](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data). Then extract the data to `data/fer2013` folder.

It's is import that modifying the `MODE`(in `main.py`) from `demo` to `train`  before you start training.
Then type:
​```shell
python3 main.py
```

#### Issues & Suggestions
If any issues and suggestions to me, you can create an [issue](https://github.com/xionghc/Facial-Expression-Recognition/issues/).

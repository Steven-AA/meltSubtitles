# Melt subtitles(融化字幕)

[只留字幕中的生词，并翻译](https://zhuanlan.zhihu.com/p/25854872)

## 思路
    1. 词库假定是你认识的单词
    2. 将字幕中在单词中的单词去掉，
    3. 通过查询有道网页得到生词的释义
    4. 将释义加入到新的字幕文件中，
    5. done

## 安装和使用
0. 安装python 2.7.9 以上，推荐[python 3.5](https://www.python.org/downloads/release/python-353)
1. pip install -r requirements.txt 
2. python main.py zimu.srt

   如果指定单词库，单词库在文件夹wordsRepo, 加上"-w wordsRepo/文件", 默认使用5000的。
   
   或者对多个字幕转换 python main.py *.srt 
   
   如果希望是英文释义，在命令行加上 "-e"

## 词库有[5000](http://www.wordfrequency.info/free.asp),[10000](https://github.com/first20hours/google-10000-english)


## To do 
1. [x] 英文释义选择

2. [x] 批量转换

3. [ ] 可以放到一个网页，使用的人可以不用安装python，只需上传下载。
4. [ ] 可以用map函数式的思想减少for的使用

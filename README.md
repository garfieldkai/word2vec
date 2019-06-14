# word2vec
word2vec训练过程及语料

## 语料准备
1、下载搜狗训练语料

下载路径：http://www.sogou.com/labs/resource/cs.php。由于只是测试word2vec的训练过程，只是下载迷你版数据，放置于data文件夹下；

2、解压语料

tar -zxvf news_sohusite_xml.smarty.tar.gz

3、修改字符集，提取内容

`cat news_sohusite_xml.smarty.dat | iconv -f gbk -t utf-8 -c | grep "<content>" > corpus.txt`
这样就生成了utf-8格式的正文内容

4、语料分词


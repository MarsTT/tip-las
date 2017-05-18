TIP-LAS: An open source toolkit for Tibetan word segmentation and part of speech tagging
===============
TIP-LAS藏文分词标注系统使用文档
===============
# 简介

分词、词性标注是自然语言处理任务的基础，应用非常广泛，为方便研究者进行对比研究，我们把分词、词性标注系统予以  开源，便于快速构建实验系统。
TIP- LAS系统基于感知机算法构建，分为分词、词性标注两大模块，分词采用统一标记集对音节和紧缩词进行标注，词性标注融合音节特征，具有领域无关等特点。

# 编译TIP-LAS 

　　Linux  下编译：进入主文件目录，输入”make”即可 
  
　　Windows下编译：在主文件目录下，用VS 2013打开“tip-las.vcxproj”文件即可
# 使用可执行程序

编译成功后，会在主目录文件夹下生成如下可执行程序: tip-las

训练命令：tip-las train  ws/pos  input  model 

说明：

train表示程序执行训练命令，ws、pos分别表示选择训练分词或者是词性标注模型，input表示输入训练文件，model表示模型文件。当选择ws或pos时，后面的输入文件需要对应切分好的分词语料，或者是词性标注语料。

测试命令：tip-las test  ws/pos/all  input  output

说明：

test表示程序执行测试命令，ws、pos、all分别表示选择测试分词、词性标注、分词标注一体，input表示输入测试文件，output表示测试结果文件。当选择ws时，输入的是纯藏文分本，输出切分好的藏文文本；当选择pos是输入的是切分好的藏文分本，输出标注结果文本；当选择all是输入的是纯藏文分本，输出的是分词、标注结果。

# 参考文献

[1]李亚超, 江静, 加羊吉,等. TIP-LAS:一个开源的藏文分词词性标注系统[J]. 中文信息学报, 2015, 29(6):203-207.

[2]李亚超, 加羊吉, 宗成庆,等. 基于条件随机场的藏语自动分词方法研究与实现[J]. 中文信息学报, 2013, 27(4):52-58.

[3]于洪志, 李亚超, 汪昆,等. 融合音节特征的最大熵藏文词性标注研究[J]. 中文信息学报, 2013, 27(5):160-165.
# Q&A
如果问题请联系：Email:harry_lyc(at)foxmail(dot)com

# 卷积神经网络

### 卷积运算方式
* 1.以随机的方式产生filter weight， 大小是3x3
* 2.在要转换的图片上由左到右，由上到下，依顺序选取3x3的矩阵
* 3.图片中选取的3x3的矩阵与filter weight做乘积，计算生成第1行、第1列的数字
  ![输入图片说明](https://github.com/xxbb1234021/deep-learning/blob/master/img/cnn_1.png "在这里输入图片标题")
* 4.以相同的方式计算生成第1行、第2列的数字
  ![输入图片说明](https://github.com/xxbb1234021/deep-learning/blob/master/img/cnn_2.png "在这里输入图片标题")
* 依照上面的方式，完成所有的计算
  

### Max-pool运算方式
* 1.Max-pool运算可以将图片缩减取样，如下图：原本图片是4x4，经过Max-pool运算后，图片大小为2x2
* 2.左上角4个数字：5,2,4,1最大的是5，所以计算结果是5
  ![输入图片说明](https://github.com/xxbb1234021/deep-learning/blob/master/img/cnn_3.png "在这里输入图片标题")
* 3.右上角4个数字是3,1,1,6最大的是6，所以计算结果是6
  ![输入图片说明](https://github.com/xxbb1234021/deep-learning/blob/master/img/cnn_4.png "在这里输入图片标题")
* 4.左下角4个数字是7,8,1,1最大值是8，所以计算结果是8
  ![输入图片说明](https://github.com/xxbb1234021/deep-learning/blob/master/img/cnn_5.png "在这里输入图片标题")
* 5.右下角4个数字是2,9,1,1最大值是9，所以计算结果是9
  ![输入图片说明](https://github.com/xxbb1234021/deep-learning/blob/master/img/cnn_6.png "在这里输入图片标题")

### Max-pool的好处
* 减少需要处理的信息量
* 图片的差异变小
* 参数的数量和计算量减小

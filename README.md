# Recommendation_System_Test
# 利用Python实现推荐系统功能
本项目实例旨在实现一个电影的推荐系统，数据来源为http://grouplens.org/datasets/movielens/  
# 运行环境
Windows7x64 + python3.5 + jupyter notebook  
# 源码及数据说明
源码：基于用户的电影推荐系统代码、基于物品的电影推荐系统代码  
数据：data/ml-100k.zip（解压后获得本实例用到的u.data和u.item两个文件）  
Base_User.ipynb主要实现的是基于用户相似度的推荐，依据信息是多个用户对同一部电影的评分，即用户间的交集，交集越多越容易推荐  
Base_Item.ipynb主要实现的是基于电影相似度的推荐，依据信息是同一个用户所有看过的电影的属性及评分，来实现在其他该用户没看过的电影中推荐他可能喜欢的电影  
其中相似度参数分为欧式距离和皮尔逊系数，在本实例中分别作了定义和计算  
u.item中的类似|0|0|0|0|0|1|0|0|0|0|0|0|0|0|0|0|0|0|0的字符串已对电影属性做了量化标注，便于数据处理与矩阵运算  
# 运行方法
打开jupyter notebook工具
创建一个项目文件夹
将源码及数据文件拷贝至项目文件夹下
分别运行Base_User.ipynb和Base_Item.ipynb，会得到如下结果：
![image](https://github.com/bestpower/Recommendation_System_Test/blob/master/readme_image_folder/result1.PNG)  
![image](https://github.com/bestpower/Recommendation_System_Test/blob/master/readme_image_folder/result2.PNG)  

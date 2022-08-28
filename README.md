# 智慧课堂学生行为数据集<br/>
## 数据集来源
数据来源：国家资源公共服务平台2019年度小学语文1-6年级部级优课的课堂实录视频<br/>
国家资源公共服务平台网址：`https://jpk.eduyun.cn/portal/html/1s1k/index/1.html`<br/>
## 数据集用途
智慧课堂学生行为数据集仅限于学术研究使用，___禁止商业应用和其他用途___。<br/>
## 数据集构成
#### 智慧课堂学生行为数据集按拍摄角度分为正面视角、斜上方视角、后方视角、教师视角<br/>
![智慧课堂采集数据的四类视角](https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/智慧课堂采集数据的四类视角.png)  
#### 数据集具体指标如下：
| 维度 | 片段数 | 时长分布（s） | 总大小 | 视频尺寸 | 帧速率 |
| :----: | :----: | :----: | :----: | :----: | :----: |
| 正方视角 | 593 | 1-174 | 574M | 800×450 | 25f/s |
| 斜上方视角 | 4781 | 1-115 | 5.30G | 800×450 | 25f/s |
| 后方视角 | 4544 | 1-59 | 3.48G | 800×450 | 25f/s |
| 教师视角 | 2918 | 1-106 | 1.93G | 800×450 | 25f/s |
## 正方视角数据集标注情况
#### 正方视角学生行为分类图例  
![学生行为分类图例](https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/学生行为分类图例.png)  
#### 正方视角下的学生行为数据集标注如下：
<table>
	<tr>
	    <th>维度</th>
	    <th>行为分类</th>
	    <th>行为描述</th> 
 	    <th>编码</th> 
	    <th>标注数量</th> 
	</tr >
	<tr >
	    <td rowspan="8">个体行为</td>
	    <td>低头写字</td>
	    <td>低头拿笔在书本上写字</td>
	    <td>dx</td>
	    <td>72462</td>
	</tr>
	<tr>
	    <td>低头看书</td>
	    <td>低头目光看向书本</td>
	    <td>dk</td>
	    <td>58932</td>
	</tr>
	<tr>
	    <td>抬头听课</td>
	    <td>抬头目光看向黑板</td>
	    <td>tt</td>
	    <td>117528</td>
	</tr>
	<tr>
	    <td>转头</td>
	    <td>向左或向右转头</td>
	    <td>zt</td>
	    <td>5339</td>
	</tr>
	<tr>
	    <td>举手</td>
	    <td>手臂抬起</td>
	    <td>js</td>
	    <td>4183</td>
	</tr>
	<tr>
	    <td>站立</td>
	    <td>全身挺直、手臂向下</td>
	    <td>zl</td>
	    <td>4101</td>
	</tr>
	<tr>
	     <td>走动</td>
	    <td>在教室中行走、奔跑</td>
	    <td>zd</td>
	    <td>0</td>
	</tr>
	<tr>
	    <td>异常状态</td>
	    <td>打哈欠、坐姿异常</td>
	    <td>yc</td>
	    <td>0</td>
	</tr>
	<tr>
	    <td rowspan="2">团队行为</td>
	    <td>小组讨论</td>
	    <td>同桌或前后桌面对面讨论</td>
	    <td>xt</td>
	    <td>4663</td>
	</tr>
	<tr>
	    <td>教师指导</td>
	    <td>教师在学生旁边指导</td>
	    <td>jz</td>
	    <td>680</td>
	</tr>
</table>

## 数据集训练
使用yolov5训练正方视角数据集，训练轮次（epco）=300，使用yolov5s模型  
#### 训练结果如下：
<img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/F1_curve.png" width="450" height="300"><img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/PR_curve.png" width="450" height="300"/>  
<img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/P_curve.png" width="450" height="300"><img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/R_curve.png" width="450" height="300"/>  
<img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/labels.jpg" width="450" height="450"><img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/labels_correlogram.jpg" width="450" height="450"/>   
<img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/results.png" width="900" height="450">  
<img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/confusion_matrix.png" width="600" height="450">  
#### 测试效果如下：
<img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/train_batch2.jpg" width="450" height="450"><img src="https://github.com/GX1300/Smart-Classroom-Student-Behavior-Dataset/blob/main/Picture/train_batch0.jpg" width="450" height="450"/>   
## 数据集下载地址
百度云地址：`https://pan.baidu.com/s/1uSdGbXAyZKbxD4fQdOrZzA?pwd=1234`  提取码：1234<br/>




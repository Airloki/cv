# cv
Something about what I knew


一.MYDB
	简介：实现python与Mysql之间金融数据互通的函数。
	主要库：pymysql tushare
	（1）update_hs300:
			抓取沪深300所有成分股的日价格数据保存到mysql数据库。
	（2）df_of_stock:
			读取数据库中某支股票的数据并生成一张DataFrame表格。
	
二.myfun01
	简介：部分金融数据指标的计算
	主要库：pandas numpy
	（1）get_atr:
			计算一段时间内价格的真实波幅atr（average true range ）。
	（2）get_CE：
			计算一段时间内价格的chandelier指标，返回chandelier long与chandelier short两组数列。
	（3）get_SMA：
			计算一段时间内价格的简单移动平均线SMA（Simple MA）。
	（4）get_boll：
			计算一段时间价格的布林线Boll,返回up band、mid band、low band三组数列
			
三.myfun02
	简介：部分金融数据指标的计算，和01运行要调用的库不同
	主要库：pandas numpy tushare
	（1）get_eps:
			抓取全部股票指定年份的eps数据并返回
	（2）get_pe:
			根据抓取的eps计算动态pe
			
四.Ridge Regression
	简介：使用机器学习中的岭回归方法构建的一个预测股价的模型
	功能：根据交易日当天的数据以及指标预测第二天的价格
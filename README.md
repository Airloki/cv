# cv
Something about what I knew


一.MYDB
	简介：实现python与Mysql之间金融数据互通的函数。
	主要库：pymysql tushare
	（1）update_hs300:
			抓取沪深300所有成分股的日价格数据保存到mysql数据库。
	（2）df_of_stock:
			读取数据库中某支股票的数据并生成一张DataFrame表格。
	
二.myfun
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
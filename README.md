# zkadmin
众科软件测试存放代码的
import time   #引入时间插件
from selenium import webdriver #导入selenium驱动
browers = webdriver.Chrome()   #调用谷歌浏览器驱动
browers.get("https://www.baidu.com/")#打开百度
time.sleep(2)                          #让程序暂停5秒
browers.find_element_by_id("kw").send_keys("天气")#找到百度搜索框，并填入搜索内容
browers.find_element_by_id("su").click()         #触发搜索按钮//*[@id="su"]

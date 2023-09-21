**Selenium 自动化测试程序（Python版）**
运行环境：
- selenium web driver
- python3
- pytest
- git

配置文件：iselenium.ini
- 将配置文件复制到本地磁盘的[user.home]目录
- 填入设备的chromwebdriver文件的全路径

环境变量：
- headless：控制是否以浏览器静默模式运行测试

运行命令（allure报告形式）：
pytest -sv test/web_ut.py --alluredir ./allure-results
运行命令（Junit报告形式）： 
pytest -sv test/web_ut.py -o junit_family=xunit2 --junit-xml=iSelenium_result.xml
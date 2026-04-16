"#my"
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
import time
driver=webdriver.Edge()
driver.get("https://google.com")
time.sleep(4)
search_box=driver.find_element(By.NAME,"q")
search_box.send_keys("Selenium")
search_box.send_keys(Keys.RETURN)
time.sleep(4)
driver.quit()

###
from selenium import webdriver
from selenium.webdriver.edge.service import Service
from selenium.webdriver.common.by import By
import time

service=Service("C:\\Users\\K Joshna Rani\\Downloads\\edgedriver_win64\\msedgedriver.exe")
driver=webdriver.Edge(service=service)
driver.get("https://google.com")
search_box=driver.find_element(By.NAME,"q")
print(search_box)
time.sleep(4)
driver.quit()

####


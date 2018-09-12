Beautiful Soup
==============

Beautiful Soup란?
-----------------
**BeautifulSoup는 HTML또는 XML을 파싱할 때 사용하는 파이썬 라이브러리이다.**


Beautiful Soup 설치
-------------------
    PowerShell을 실행하고
    pip intall beautifulsoup4 를 입력한다.
    
Beautiful Soup 사용법
--------------------
    1 from bs4 import BeautifulSoup
    2
    3 soup = BeautifulSoup(open("index.html"))

+파싱할 문서를 Beautiful 클래스의 생성자에 넘겨주어 문서 개체를 생성한다.

+여기서 이 문서 개체는 soup라 부른다.

    1 from bs4 import BeautifulSoup
    2
    3 soup1 = BeautifulSoup(open("index.html"), "lxml")
    4 soup2 = BeautifulSoup("<html>data</html>")

+lxml등 외부 파서를 설치한 후에도 사용할 수 있다.

    1 import requests
    2 from bs4 import BeautifulSoup
    3
    4 html = requests.get("http://www.hwanho.net")
    5 soup = BeautifulSoup(html, "lxml")
    
+urllib 또는 Requests 모듈을 함께 사용하여 그 url의 HTML을 파싱할 수도 있다.

    1 import requests
    2 from bs4 import BeautifulSoup
    3
    4 res = requests.get("https://news.v.daum.net/v/20180911171941726")
    5 res.encoding = "utf-8"
    6 soup = BeautifulSoup(res.text)
    7 postTitles = soup.find_all(class_="entry-title")
    8
    9 for postTitle in postTitles:
    10     print(postTitle.text)
    




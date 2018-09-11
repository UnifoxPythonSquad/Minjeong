Beautiful Soup
==============

Beautiful Soup란?
-----------------
**BeautifulSoup는 HTML또는 XML을 파싱할 때 사용하는 파이썬 라이브러리이다.**


Beautiful Soup 설치
-------------------
    PowerShell을 실행하고
    $ pip intall beautifulsoup4 를 입력한다.
    
Beautiful Soup 사용법
--------------------
    1 from bs4 import BeautifulSoup
    2 soup = BeautifulSoup(open("index.html"))

+파싱할 문서를 Beautiful 클래스의 생성자에 넘겨주어 문서 개체를 생성한다.

+여기서 이 문서 개체는 soup라 부른다.




# 데이터 수집
### 크롤링(crawling) 기본
① 라이브러리 임포트</br>
import requests </br>
from bs4 import BeautifulSoup </br>
</br>
② 웹 페이지 가져오기 </br>
res = requests.get('도메인 주소') </br>
</br>
③ 웹 페이지 파싱하기 </br>
soup = BeautifulSoup(res.content, 'html.parser') </br>
</br>
④ 필요한 데이터 추출하기 </br>
mydata = soup.find('태그') </br>
print(mydata.get_text())

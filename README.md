# 최양선 할머님의 팔순 생신 잔치 초대장 홈페이지 소스입니다.
최양선 할머님의 생신 잔치에 초대합니다.

소스 코드 출처 : https://github.com/hanbyeol-sungsub-wedding/hanbyeol-sungsub-wedding.github.io

생신 잔치 후기 : 차후 URL 공유 예정


# 클릭 이벤트와 스크롤 추적 하는 법

1. [Google Analytics](https://analytics.google.com) 코드 설치
2. 링크 클릭 이벤트 
    
```html
<a onclick="ga('send', 'event', '페이스북 이벤트 페이지', '링크 클릭');" 
href="https://www.facebook.com/events/153683578462761/" >페이스북 이벤트에 댓글 달기</a>
```
  
3. 사진 클릭 이벤트 

```html
<a onclick="ga('send', 'event', '갤러리', '클릭', '긴 하루의 끝');" href="./images/g9.jpg" 
class="magnific-zoom-gallery" title="긴 하루의 끝">
```

4. 스크롤 추적 이벤트: 라이브러리 http://scrolldepth.parsnip.io/

> 화면의 25%, 50%, 75%, 100% 읽은 사람의 숫자를 google analytics에 보낸다.

```html
<script src="js/jquery.scrolldepth.min.js"></script>
<script>
jQuery(function() {
  jQuery.scrollDepth();
});
</script>
```

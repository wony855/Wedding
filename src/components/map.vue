<template>
  <div class="container">
    <br>
    <div class="title">
      <p>오시는 길</p>
    </div>
    <div class="locationTitle">
      <p>웨딩바이이명원</p>
    </div>
    <div class="location">
      <p>대구 남구 안지랑로 15 (2층)</p>
      <p>TEL. 0507-1314-8009</p>
    </div>
    
    <div class="wedding-map" style="font: 12px AppleSDGothicNeo-Regular, dotum, sans-serif; letter-spacing: -1px; width: 96%; max-width: 520px; height:auto; color: rgb(51, 51, 51); position: relative; left: 50%">
      <div style="width: 96%; max-width: 520px; height:auto">
        <a href="https://map.kakao.com/?urlX=854907&amp;urlY=651603&amp;itemId=50158094&amp;q=%EC%9B%A8%EB%94%A9%EB%B0%94%EC%9D%B4%EC%9D%B4%EB%AA%85%EC%9B%90&amp;srcid=50158094&amp;map_type=TYPE_MAP&amp;from=roughmap" target="_blank">
          <img class="map" src="http://t1.daumcdn.net/roughmap/imgmap/f2be7b5bf1a0e1ae4987b784c5df56dc2be9ce68d05d104adb47a4c16f8abfbb" width=99.5% height=99.5% style="border: 1px solid rgb(204, 204, 204);">
        </a>
      </div>
      <div style="overflow: hidden; padding: 7px 11px; margin: -5px 0; border: 1px solid rgba(0, 0, 0, 0.1); border-radius: 0px 0px 2px 2px; background-color: rgb(249, 249, 249);">
        <a href="https://map.kakao.com?map_type=TYPE_MAP&amp;from=roughmap&amp;srcid=50158094&amp;itemId=50158094&amp;q=%EC%9B%A8%EB%94%A9%EB%B0%94%EC%9D%B4%EC%9D%B4%EB%AA%85%EC%9B%90&amp;urlX=854907&amp;urlY=651603" target="_blank" style="float: left;">
          <img src="//t1.daumcdn.net/localimg/localimages/07/2018/pc/common/logo_kakaomap.png" width="72" height="16" alt="카카오맵" style="display:block;width:72px;height:16px">
        </a>
        <div style="float: right; position: relative; top: 1px; font-size: 11px;">
          <a target="_blank" href="https://map.kakao.com/?from=roughmap&amp;srcid=50158094&amp;confirmid=50158094&amp;q=%EC%9B%A8%EB%94%A9%EB%B0%94%EC%9D%B4%EC%9D%B4%EB%AA%85%EC%9B%90&amp;rv=on" style="float:left;height:15px;padding-top:1px;line-height:15px;color:#000;text-decoration: none;">로드뷰</a>
          <span style="width: 1px;padding: 0;margin: 0 8px 0 9px;height: 11px;vertical-align: top;position: relative;top: 2px;border-left: 1px solid #d0d0d0;float: left;"></span>
          <a target="_blank" href="https://map.kakao.com/?from=roughmap&amp;eName=%EC%9B%A8%EB%94%A9%EB%B0%94%EC%9D%B4%EC%9D%B4%EB%AA%85%EC%9B%90&amp;eX=854907&amp;eY=651603" style="float:left;height:15px;padding-top:1px;line-height:15px;color:#000;text-decoration: none;">길찾기</a>
          <span style="width: 1px;padding: 0;margin: 0 8px 0 9px;height: 11px;vertical-align: top;position: relative;top: 2px;border-left: 1px solid #d0d0d0;float: left;"></span>
          <a target="_blank" href="https://map.kakao.com?map_type=TYPE_MAP&amp;from=roughmap&amp;srcid=50158094&amp;itemId=50158094&amp;q=%EC%9B%A8%EB%94%A9%EB%B0%94%EC%9D%B4%EC%9D%B4%EB%AA%85%EC%9B%90&amp;urlX=854907&amp;urlY=651603" style="float:left;height:15px;padding-top:1px;line-height:15px;color:#000;text-decoration: none;">지도 크게 보기</a>
        </div>
      </div>
    </div>
    <br>
    <br>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  max-width: 768px;
  margin:0 auto;
}
.title p {
  font-size: 2.25rem;
  margin: 0 auto;
  padding-left: 1.5rem;
  padding-bottom: 3rem;
  letter-spacing: 0.6rem;
  text-align: center;
}
.locationTitle p {
  font-size: 1.8rem;
  text-align: center;
  font-weight: bold;
}
.location p {
  font-size: 1.6rem;
  text-align: center;
  padding-bottom: 1rem;
  margin: 0;
}
.wedding-map {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
}
@keyframes fadein {
  0%{
    opacity: 0;
  }
  100%{
    transition: opacity 0.3s;
  }
}
@keyframes fadeout {
  from{
    opacity: 1;
  }
  to{
    opacity: 0;
  }
}
</style>

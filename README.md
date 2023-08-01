# jemam
예맘 입학 홍보
<html>
<head>
<title>카카오톡 버튼있는 메시지 전송하기</title>
<script id="javascript-sdk" src="https://developers.kakao.com/sdk/js/kakao.min.js"></script>
</head>
<body>
<p><strong>아래 카카오톡 아이콘을 눌러 전송하세요</strong> By. Jesang</p>
<a id="kakao-link-btn" href="javascript:sendLink()">
  <img
    src="https://developers.kakao.com/assets/img/about/logos/kakaolink/kakaolink_btn_medium.png"
  />
</a>
<script type="text/javascript">
 Kakao.init('3a548625cfdf4b67bdb86a3c0f7cfbb5');
  function sendLink() {
    Kakao.Link.sendDefault({
      objectType: 'feed',
      content: {
        title: '상담목회 아카데미 예맘',
        description: '신입생을 모집합니다.',
        imageUrl:
          'https://drive.google.com/file/d/1yWCgGhpgRwrtrgEaforl4rtn-zsn9pXl',
        link: {
          mobileWebUrl: 'https://www.jemam.org',
          webUrl: 'https://www.jemam.org',
        },
      },
      social: {
        likeCount: 99999, //99999가 최대입니다
        commentCount: 99999, //99999가 최대입니다
        sharedCount: 99999, //99999가 최대입니다
      },
      buttons: [
        {
          title: '자세히 알아 보기',
          link: {
            mobileWebUrl: 'https://www.jemam.org',
            webUrl: 'https://www.jemam.org',
          },
        },
      ],
    })
  }
</script>
<!-- www.blackcats4567.com -->
<!-- 이미지/버튼 클릭 시 주소는 Kakao Developers의 애플리케이션 > 플랫폼 > Web에 넣어야 클릭했을때 성공적으로 표시됩니다 -->
  </body>
</html>

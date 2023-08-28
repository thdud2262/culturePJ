# 나-도 문화인
### 공연 정보를 한번에 보고 싶은 사람들을 위한 서비스
평소 문화 공연에 관심이 많은 사람들을 위한 서비스를 제작해보았습니다. 저는 음악회를 보고 싶을 때면 예술의 전당 홈페이지를 들어가 마음에 드는 공연을 찾아봅니다. 하지만 전시회나 공연을 보고 싶을 때는 검색엔진으로 검색해 봐야 했던 것에 약간의 불편함을 느껴서 공공API를 활용해 문화 공연 정보를 알려주는 서비스를 만들어보고 싶다는 생각이 들었습니다.<br>
<br>
<br>

## 🍎 배포 링크 Hosting URL, 개발 기간
### https://culture-me.vercel.app/
- version_01 개발기간 : 2023/07/03 - 2023/08/06 
<br>
<br>

## 🍋 구현 내용 (version_01)
- Next.js 13의 가장 큰 특징인 **파일 시스템을 기반으로 한 라우팅을 사용**하였습니다. 파일과 폴더를 정의하여 정적 및 동적 라우팅을 구현하여 페이지를 만들었습니다.
- **loading, error 등의 상태를 처리**하여 사용자가 페이지에서 어떤 일이 발생하는지 알 수 있도록 하였습니다.
- Next.js에서는 서버 / 클라이언트 두 종류의 컴포넌트가 있습니다. **두 컴포넌트의 차이점과 이를 사용해야 하는 경우를 공부하며 각 페이지의 컴포넌트를 적용**하였습니다.
- **Next.js의 서버에서 공공API데이터를 요청하여 데이터를 사용**하였습니다. 클라이언트에서 데이터를 요청하지 않고, 서버로 이동하여 서버에서 공공API데이터를 요청하였고, 이를 클라이언트로 넘겨주어 사용자가 데이터를 볼 수 있도록 하였습니다. 공공API데이터를 최적화 할 수 있는 방법을 더 공부하고 있습니다.
- 공공API데이터의 **키워드에 해당하는 공연 정보를 볼 수 있게 하였고, 검색 기능**도 구현하였습니다
- 랜덤으로 들어오는 **공공API데이터를 sort, filter하는 util함수를 구현**하여 코드를 중복작성 하지 않고, 필요한 페이지마다 import하여 사용할 수 있도록 하였습니다. 
- **calendar를 직접 구현**하여 사용자가 날짜별로 공연 정보를 더욱 쉽게 볼 수 있도록 하였습니다.
<br>
<br>

## 🍊 프로젝트 세팅
#### 설치하기 Installation
```bash
> npm install
```

#### 개발 모드로 실행하기
```bash
> npm run dev
```

#### 프로덕션 모드로 실행하기
```bash
> npm run build   // 빌드 후
> npm start       // 프로젝트 실행
```
<br>
<br>

## 🍏 기술스택 Project Stack

- javascript
- next.js
  <br>
  <br>


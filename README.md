# 성수 팝업스토어 (seongsu-popupstore)

한국노총 성수유니온랩의 온라인 팝업스토어와 익명 카톡 라운지 연결 페이지입니다.

## 주소 구조
- `/` 팝업스토어 본 페이지 (메뉴판 · 계산기 · 장바구니)
- `/lounge` 익명 카톡방으로 자동 연결되는 중간 페이지

## 인쇄물 QR 주소 (배포 주소가 seongsu-popupstore.vercel.app일 때)
- 책갈피 뒷면 → `https://seongsu-popupstore.vercel.app/?src=bookmark`
- 부적 뒷면 → `https://seongsu-popupstore.vercel.app/lounge?src=charm`
- 너도 그래? 보드 → `https://seongsu-popupstore.vercel.app/?src=board`
- 영수증 핸드아웃 → `https://seongsu-popupstore.vercel.app/?src=receipt`

## 카톡방이 바뀌면
`lounge/index.html`의 `LOUNGE_URL` 한 줄과 `noscript` · 버튼의 기본 주소만 바꾸면 됩니다. 인쇄된 QR은 그대로 씁니다.

## 배포
1. GitHub에 새 저장소 `seongsu-popupstore`를 만들고 이 폴더의 파일을 모두 올립니다.
2. Vercel → Add New → Project → 저장소 선택 → Framework Preset은 Other → Deploy.
3. 배포 주소를 확인합니다. 이름이 이미 쓰이고 있으면 다른 주소가 나오니 그 주소로 QR을 다시 만듭니다.

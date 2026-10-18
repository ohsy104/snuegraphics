# snuegraphics

AI 세계 기후 탐험대 웹사이트입니다.

- Teachable Machine 모델을 사용해 기후 이미지를 분류합니다.
- 사진 업로드 후 예측 결과를 확인할 수 있습니다.
- 신뢰도가 75% 미만이면 "불확실"로 처리합니다.
- 혼동행렬을 기반으로 정답/오답을 시각화합니다.
- 오답 이미지 갤러리와 정확도 통계를 제공합니다.

## 실행 방법

로컬에서 확인하려면 브라우저에서 `index.html`을 직접 열면 됩니다.

```bash
python -m http.server 8000
```

그 다음 브라우저에서 다음 주소로 접속합니다.

```text
http://localhost:8000
```

## Vercel 배포

1. 이 저장소를 GitHub에 푸시합니다.
2. Vercel에 접속합니다.
3. "Add New Project"를 선택합니다.
4. 이 저장소를 import 합니다.
5. 프레임워크는 기본값을 유지하고, 빌드 명령은 비워 둡니다.
6. 프로젝트를 배포합니다.

이 프로젝트는 정적 HTML 파일 기반이라 별도 빌드 단계가 필요하지 않습니다.

## 참고

- Teachable Machine 모델 URL: https://teachablemachine.withgoogle.com/models/4E3fH9sQf/
- 구현 파일: `index.html`

# 무인아이스크림 관리 앱 - GitHub Pages 배포용

이 폴더는 GitHub Pages에 바로 올릴 수 있는 정적 사이트 버전입니다.

## 포함 파일
- `index.html` : 앱 본체
- `.nojekyll` : GitHub Pages 정적 파일 처리용

## 배포 방법

### 방법 1) GitHub 웹사이트에서 바로 업로드
1. GitHub에서 새 저장소(repository)를 만듭니다.
   - 예: `icecream-manager`
2. 이 폴더 안의 파일(`index.html`, `.nojekyll`)을 저장소 루트에 업로드합니다.
3. GitHub 저장소에서 **Settings > Pages**로 이동합니다.
4. **Build and deployment**에서:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
5. 저장하면 몇 분 뒤 배포 주소가 생성됩니다.
   - 예: `https://<github-username>.github.io/icecream-manager/`

### 방법 2) GitHub Desktop 사용
1. 새 저장소를 만듭니다.
2. 이 폴더의 파일을 저장소 폴더에 복사합니다.
3. Commit 후 Push 합니다.
4. GitHub 웹사이트에서 **Settings > Pages**로 들어가 위와 같이 설정합니다.

## 사용 시 주의
- 데이터는 브라우저의 `localStorage`에 저장됩니다.
- 다른 PC/브라우저로 자동 동기화되지 않습니다.
- 중요한 데이터는 앱 상단의 **전체 백업** 버튼으로 JSON 파일 저장을 권장합니다.

## 추천 운영 방식
- 평소: 앱에서 직접 입력
- 대량 데이터: 엑셀/CSV 업로드
- 매일 마감 후: 전체 백업
- 월말: 손익 CSV 다운로드

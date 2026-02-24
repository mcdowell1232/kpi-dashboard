[README.md](https://github.com/user-attachments/files/25516409/README.md)
# 🤖 마케팅 KPI 모니터링 대시보드

로봇청소기 키워드 검색량 일간 추이 분석 대시보드

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat&logo=chartdotjs&logoColor=white)

---

## 🎯 주요 기능

### 📊 4개 라인 차트
1. **25 vs 26 로봇청소기** - 연도별 검색량 비교
2. **25 vs 26 로보락** - 브랜드 인지도 변화
3. **S9 vs S10 Max V Ultra** - 제품 모델별 추이
4. **경쟁사 분석** - S10 (로보락), 삼성, 드리미X60, 에코백스T90

### ✨ 특징
- 📅 **날짜 필터** - 기간 선택 가능 (기본: 2026-01-01 ~ 2026-04-08)
- 🔄 **실시간 데이터** - 구글 시트 연동 (자동 갱신)
- 🎨 **브랜드 컬러** - 로보락(빨강), 삼성(진한 파랑), 드리미(연한 파랑), 에코백스(갈색)
- 📈 **곡선 처리** - 부드러운 라인 차트 (tension: 0.4)
- 💫 **0값 처리** - 검색량이 0인 날짜는 선이 끊어짐 (spanGaps: false)

---

## 🚀 데모

**🔗 Live Demo**: [https://mcdowell1232.github.io/kpi-dashboard/](https://mcdowell1232.github.io/kpi-dashboard/)

---

## 📦 설치 및 사용

### 로컬 실행
```bash
# 1. 저장소 클론
git clone https://github.com/mcdowell1232/kpi-dashboard.git
cd kpi-dashboard

# 2. 브라우저에서 열기
# index.html 파일을 더블클릭하거나

# 3. 로컬 서버 실행 (선택)
python -m http.server 8000
# 브라우저에서 http://localhost:8000 접속
```

### GitHub Pages 배포
1. GitHub 저장소 생성
2. `index.html` 업로드
3. Settings → Pages → Branch: main → Save
4. 1-2분 후 자동 배포 완료!

---

## 🔧 기술 스택

| 기술 | 용도 |
|------|------|
| **Chart.js** | 라인 차트 렌더링 |
| **Luxon** | 날짜/시간 처리 |
| **PapaParse** | CSV 파싱 |
| **All Origins CORS Proxy** | CORS 우회 |

---

## 📊 데이터 소스

- **구글 시트**: CSV 형식으로 퍼블리시
- **자동 갱신**: 구글 시트 수정 → 페이지 새로고침

### 데이터 업데이트 방법
1. [구글 시트 열기](https://docs.google.com/spreadsheets/d/e/2PACX-1vTYbyHRNM0Mtm47UkGFPSaHA0vVJER1imwpttDebMaJHr1jqDgL-P3eI7POuMYpKQ/edit)
2. 데이터 수정 후 저장
3. 대시보드에서 **"🔄 데이터 새로고침"** 버튼 클릭

---

## 🎨 차트 색상

```javascript
로보락 (S10, 26 로보락): rgb(220, 38, 38)  // 빨강
삼성 로봇청소기: rgb(30, 64, 175)           // 진한 파랑
드리미 X60: rgb(96, 165, 250)              // 연한 파랑
에코백스 T90: rgb(120, 53, 15)             // 갈색
25 로봇청소기: rgb(59, 130, 246)            // 파랑
26 로봇청소기: rgb(239, 68, 68)             // 빨강
25 로보락: rgb(34, 197, 94)                // 초록
S9 Max V Ultra: rgb(249, 115, 22)         // 오렌지
```

---

## 💡 주요 업데이트

### v1.1.0 (2026-02-24)
- ✨ **0값 선 끊기 기능** 추가
  - 검색량이 0인 날짜는 선이 끊어짐
  - `spanGaps: false` 옵션 적용
- 🔧 `cleanNumber()` 함수 개선
  - 0 → null 변환

### v1.0.0 (2026-02-24)
- 🎉 초기 배포
- 📊 4개 라인 차트 구현
- 🔄 구글 시트 연동
- 📅 날짜 필터 기능

---

## 📝 파일 구조

```
kpi-dashboard/
├── index.html          # 메인 대시보드 (18KB)
├── README.md           # 이 파일
└── UPDATE_NOTES.md     # 상세 업데이트 노트
```

---

## 🐛 알려진 제한사항

- CORS 프록시 사용으로 초기 로딩 약간 느림 (1-2초)
- 구글 시트가 비공개 상태면 접근 불가
- 인터넷 연결 필요 (CDN 사용)

---

## 🤝 기여

버그 리포트나 기능 제안은 [Issues](https://github.com/mcdowell1232/kpi-dashboard/issues)에 등록해주세요!

---

## 📄 라이선스

MIT License

---

## 👤 작성자

**mcdowell1232**
- GitHub: [@mcdowell1232](https://github.com/mcdowell1232)

---

## 📞 문의

프로젝트에 대한 질문이나 제안사항이 있으시면 GitHub Issues를 이용해주세요.

---

**⭐ 이 프로젝트가 유용하다면 Star를 눌러주세요!**

---

Made with ❤️ for Marketing Analytics

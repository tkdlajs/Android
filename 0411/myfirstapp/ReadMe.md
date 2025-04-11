# 📱 MyRoutineApp – 하루 루틴 안드로이드 앱

> 집중력 향상 + 목표 관리 + 다크모드 설정까지 가능한 실속형 앱 🎯  
> **총 5개의 액티비티로 구성되어 있으며, 데이터베이스 없이 SharedPreferences만으로 모든 기능을 구현했습니다.**

---

## ✅ 주요 기능

| 기능 번호 | 액티비티 이름        | 설명 |
|-----------|---------------------|------|
| 1️⃣        | MainActivity1       | 앱 메인화면 – 각 기능으로 이동하는 메뉴 |
| 2️⃣        | MainActivity2       | 집중 타이머 (25분 타이머 / 정지 / 초기화 / 자동 기록 저장) |
| 3️⃣        | MainActivity3       | 다크모드 설정 (스위치로 ON/OFF, 앱 전체 테마 적용) |
| 4️⃣        | MainActivity4       | 공부 기록 보기 (타이머 종료 시 시간 저장 → 목록 출력) |
| 5️⃣        | MainActivity5       | 오늘의 목표 여러 개 작성 / 완료 체크 / 삭제 가능 |

---

## 🧱 프로젝트 구조

```
📁 java/com.example.myroutineapp/
├── MainActivity1.java    ← 메인 메뉴
├── MainActivity2.java    ← 집중 타이머
├── MainActivity3.java    ← 다크모드 설정
├── MainActivity4.java    ← 공부 기록 보기
├── MainActivity5.java    ← 오늘의 목표 (리스트)
├── GoalItem.java         ← 목표 데이터 모델
├── GoalAdapter.java      ← 목표 리스트 어댑터 (완료 / 삭제 처리)
```

```
📁 res/layout/
├── activity_main1.xml    ← 메인 UI
├── activity_main2.xml    ← 타이머 UI
├── activity_main3.xml    ← 다크모드 UI
├── activity_main4.xml    ← 공부 기록 보기 UI
├── activity_main5.xml    ← 목표 입력 + 리스트 UI
├── goal_item.xml         ← 목표 1개 표시용 커스텀 항목 UI
```

---

## 💾 데이터 저장 방식

- **SharedPreferences만 사용**
  - 목표 리스트: `goal_list` (`goal_data` key, JSON 형식)
  - 타이머 기록: `study_history`
  - 테마 상태: `theme_pref`
- 데이터베이스 없이도 앱 껐다 켜도 유지됨 ✅

---

## 🖼️ 기능 스크린샷 예시 (옵션)

> 여기에 이미지 삽입 가능:
```markdown
![메인화면](screenshots/main.png)
![타이머](screenshots/timer.png)
```

---

## 📦 사용 기술

- Java (Android SDK)
- Android Studio
- SharedPreferences
- ListView + Custom Adapter
- Layout: LinearLayout / ScrollView

---

## 🚀 향후 확장 가능 기능

- 날짜별 목표 기록 / 통계 보기
- 목표 달성률 퍼센트 표시
- Room DB / Firebase 연동
- Notification 알림 기능

---

## 👨‍💻 제작자

> Designed & Coded by [HaJaeBeom]  
> Feel free to fork or star ⭐

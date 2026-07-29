# CLAUDE.md

## 프로젝트 개요
- 무엇: Windows에서 항상 맨 앞에 떠 있는 작은 팝업으로 Claude Code의 5시간 롤링 사용량(%)을 보여주는 개인용 도구
- 스택: Python. 패키지 본체는 `claude_usage_monitor/` (ui / usage_api / provider / local_estimate / voice / autostart)
- 홈 모노레포에서 2026-07-11에 독립 리포로 분리됨

## 실행
- 실행: `run.pyw` 또는 `start.bat`
- 설치/제거: `install.bat` / `uninstall.bat` (자동시작 등록은 `autostart.py`)
- 사용법 문서: `사용설명서.md`

## 컨벤션
- 자격증명은 `credentials.py` 경로로만 다루고 리포에 값을 남기지 않는다
- Windows 전용 도구다. 경로·자동시작·트레이 동작은 Windows 기준으로만 검증한다

## 세션 규칙 (중요)
- 세션 시작 시: PROGRESS.md를 먼저 읽고 이어서 작업할 것
- 세션 종료 시: PROGRESS.md를 업데이트할 것 (한 일 / 다음 할 일 / 막힌 점)
- 머신 전환(메인 PC ↔ 노트북): 작업 시작 전 `git pull`, 자리 뜰 때 커밋 후 `git push`
- git 명령은 사람이 직접 치지 않는다. commit / push / pull 은 Claude Code가 전담한다

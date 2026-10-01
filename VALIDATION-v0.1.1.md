# Antenna Pattern Tauri v0.1.1 배포 검증 (2026-10-02)

- Cargo desktop/server, Tauri 설정, 화면/창 제목, PC INFO, 서버 버전: 0.1.1.
- Windows all-targets 테스트: 39개 통과, 실패 0개, 사용자 측정 데이터가 필요한 2개 제외.
- Windows all-targets Clippy -D warnings 및 release 빌드: 통과.
- Windows EXE 실제 기동: 응답 정상, 창 제목 Antenna Pattern Tauri v0.1.1 확인 후 종료.
- EXE FileVersion/ProductVersion: 0.1.1 / 0.1.1. 정적 CRT 및 개인 빌드 경로 재매핑 적용.
- EXE SHA-256: 01db4203cfeee320de3cc6992eb268615d5344da5cde576f615f3364063332ad
- Ubuntu 24.04에서 core/no-default-features 테스트 및 엄격한 Clippy: 통과.
- Ubuntu 서버 테스트 10개 통과. 별도 FFmpeg/ffprobe VP9→H.264 MOV 검증 1개도 통과.
- Ubuntu 서버 release 빌드 및 기존 package-ubuntu.sh 패키징: 통과.
- 패키지 압축 해제 후 내부 SHA-256 9개 항목 일치, 서버 실제 기동·healthz 버전 0.1.1·화면 제공·정상 종료 확인.
- JavaScript 문법과 녹화 실패→폐기→재시작 회귀 검사: 통과.
- Windows ZIP에는 EXE, README, 현재/과거 검증 기록과 체크섬을 포함합니다.
- Linux tar.gz에는 서버, 공개 UI, 설치/서비스 파일, README, VERSION과 체크섬만 포함합니다.
- 전체 수동 GUI·실제 사용자 측정 데이터 추가 시험과 AWS 운영 서버 배포는 수행하지 않았습니다.

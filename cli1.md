# Lecture Note: CLI (Command Line Interface) - 1

## 1. Linux
- **리눅스**: 오픈소스 Unix-like OS & 커널 (1991년 Linus Torvalds 최초 공개)  
- 주요 배포판: Debian, Fedora, Ubuntu 등  
- 서버 OS 점유율: 상위 100만 웹서버 중 96.4% 이상  
- 임베디드/모바일(Android)에도 사용  
- 오픈소스 개발의 대표 플랫폼  
- CLI 기반 실행 (일부 배포판은 GUI 지원)  
- 안정적이고 보안성 높음  

---

## 2. Kernel & Shell
- **Kernel**: 하드웨어 자원을 제어하고 OS 핵심 역할 수행  
- **Shell**: 사용자가 커널과 상호작용할 수 있도록 명령어 인터페이스 제공  
  - 예: `bash`, `zsh`  

---

## 3. CLI vs GUI
| 구분 | CLI | GUI |
|------|-----|-----|
| 입력 방식 | 키보드 명령어 | 마우스 중심 + 일부 단축키 |
| 속도 | 빠름 | 상대적으로 느림 |
| 반복 작업 | 스크립트 자동화 가능 | 수동 반복 필요 |
| 사용 대상 | 개발자 친화적 | 일반 사용자 친화적 |

---

## 4. Shell 실행 방법
- **Linux/MacOS**: 앱 검색 → "Terminal" 실행  
- **Windows**: [Git Bash](https://git-scm.com/) 설치 후 실행  

---

## 5. 주요 Shell 명령어

### (1) 경로 확인
```bash
pwd    # 현재 디렉토리 경로 출력
```

### (2) 디렉토리 이동 & 목록 확인
```bash
cd [directory]   # 디렉토리 이동
ls               # 파일/디렉토리 목록 출력
```
- 인자 (arguments)
  - / : root

  - . : 현재 디렉토리

  - .. : 상위 디렉토리

  - ~ : 홈 디렉토리

  - ./ : 상대 경로

  - /[dir] : 절대 경로

- 옵션 (options)

  - -l : 상세 정보 표시 (long format)

  - -lh: 파일 크기를 읽기 좋은 단위로 표시

### (3) 기타 기본 기능

- 자동완성: tab

- 이전 명령어 불러오기: ↑ (up arrow)

- 화면 지우기: clear

### 6. 파일/디렉토리 조작 (Manipulation)

복구 불가능할 수 있음 → 중요한 파일은 백업 필수

```bash
cp source target   # 복사
mv source target   # 이동 / 이름 변경
rm file            # 삭제 (영구적!)
mkdir dirname      # 새 디렉토리 생성
```

- 와일드카드 사용:

  - * : 모든 문자열

  - ? : 한 글자

### 7. 도움말 & 종료
```bash
help command   # 내부 명령어 도움말
man command    # 메뉴얼 페이지
exit           # 터미널 종료
```

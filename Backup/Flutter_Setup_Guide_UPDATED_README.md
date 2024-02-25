
# Flutter 개발 환경 설정 가이드 (업데이트)

이 문서는 Flutter 앱 개발을 처음 시작하는 분들을 위한 기본적인 환경 설정 순서와 관련 커맨드를 안내합니다.

## 1. 안드로이드 스튜디오 설치

- **웹사이트에서 직접 다운로드**: [Android Studio 공식 웹사이트](https://developer.android.com/studio)에서 최신 버전을 다운로드하고 설치합니다.

## 2. Flutter 설치

### macOS:

- **Brew 설치**:
  ```bash
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```

- **Flutter 설치**:
  ```bash
  brew install --cask flutter
  ```

### Windows:

- **PowerShell 설치**:
  PowerShell이 설치되어 있지 않은 경우, Microsoft 공식 웹사이트 또는 Windows Store를 통해 PowerShell을 설치하세요.

- **Choco 설치** (PowerShell 필요):
  ```powershell
  Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
  ```
  이 커맨드를 실행하기 위해서는 PowerShell이 필요하며, 설치 과정에서 네트워크 보안 프로토콜을 설정하는 단계를 포함합니다.

- **Flutter 설치**:
  ```powershell
  choco install flutter
  ```

## 3. 비주얼 스튜디오 설치

- Flutter 개발에 필요한 다양한 플랫폼을 위한 C++ 및 모바일 개발 도구를 포함하기 위해, [Visual Studio](https://visualstudio.microsoft.com/)를 설치합니다. 설치 시 **모바일 개발을 위한 .NET**과 **C++을 사용한 데스크톱 개발** 워크로드를 선택하세요.

## 4. Flutter 개발 환경 설정

- **Flutter Doctor 실행**:
  ```bash
  flutter doctor
  ```

- **Android SDK 설정**:
  Flutter는 Android 앱 개발을 위해 Android SDK가 필요합니다. Android Studio를 통해 관리할 수 있습니다.

- **안드로이드 에뮬레이터 또는 실제 디바이스 설정**:
  Android Studio의 AVD Manager를 사용하여 에뮬레이터를 생성하거나, 개발자 옵션을 활성화한 실제 Android 디바이스를 사용할 수 있습니다.

- **IDE에 Flutter 및 Dart 플러그인 설치**:
  Visual Studio Code나 IntelliJ IDEA에 Flutter와 Dart 플러그인을 설치합니다.

## 5. 첫 Flutter 앱 생성 및 실행

- **앱 생성**:
  ```bash
  flutter create my_app
  ```

- **앱 실행**:
  ```bash
  cd my_app
  flutter run
  ```

Flutter 개발 환경을 설정하고 첫 앱을 생성 및 실행하는 기본적인 단계를 소개했습니다. 개발 과정에서 문제가 발생하면, [Flutter 공식 문서](https://flutter.dev/docs)를 참조하거나 커뮤니티 포럼을 활용하세요.

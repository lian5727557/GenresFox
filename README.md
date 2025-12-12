#GenresFox
<div align="center">
https://img.shields.io/badge/version-0.3.8-blue.svg
https://img.shields.io/badge/license-MIT-green.svg
https://img.shields.io/badge/chrome-manifest%2520v3-orange.svg

完全开源、极其简洁、高度可定制的新标签页扩展

English | 中文 | 日本語 | 한국어 | Español | Français

https://assets/Screenshots/Show-1.png

</div>
English
✨ Features
🎨 Modern Dark Theme: Beautiful glassmorphism design with smooth animations

🔍 Multi-Engine Search: Built-in support for Google, Bing, and DuckDuckGo

⚙️ Custom Search Engines: Add your own search engines with custom URLs

🔖 Quick Shortcuts: Create shortcuts to your favorite websites with auto-fetched favicons

🖼️ Custom Wallpapers: Upload your own background images (up to 50MB, 50MP) with drag-and-drop support

🌅 Bing Daily Wallpaper: Beautiful daily wallpapers from Bing with smart 24-hour caching and preloading

⚡ High-Performance Image Processing: Web Worker support, progressive preview, and intelligent compression

🌍 Multi-language: English, Simplified Chinese, Traditional Chinese, Japanese, Spanish, French, Korean

♿ Accessibility: High contrast themes, font controls, animation settings, keyboard shortcuts

⌨️ Keyboard Shortcuts: Quick engine switching (Alt+↑↓), focus search (/), open settings (Alt+,)

💾 Smart Caching: Icon caching, wallpaper caching, and processing result caching for faster loading

🎯 Clean & Minimal: Distraction-free interface focused on what matters

🌐 Language Switching: Easy language switching through settings with auto-detection

🚀 Installation
From Source
Clone this repository:

bash
git clone https://github.com/zayokami/GenresFox.git
Open Chrome/Edge and navigate to chrome://extensions/

Enable "Developer mode" in the top right corner

Click "Load unpacked" and select the src folder

Enjoy your new tab page!

From Chrome Web Store
Coming soon...

🛠️ Usage
Search
Simply type in the search box and press Enter

Click the search engine icon to switch between different engines

URLs are automatically detected and opened directly

Custom Search Engines
Click the settings icon (⚙️) in the bottom right

Go to "Search & Shortcuts" tab

Enter the engine name and URL (use %s as the search query placeholder)

Example: https://kagi.com/search?q=%s

Click "Add"

Shortcuts
Open settings and go to "Search & Shortcuts" tab

Scroll to the "Shortcuts" section

Enter the name and URL of your favorite website

The favicon will be automatically fetched

Custom Wallpaper
Open settings and go to "Wallpaper" tab

Drag and drop an image or click to upload

Maximum file size: 50MB, maximum resolution: 50 megapixels

Images are automatically optimized and compressed for storage efficiency

Click "Reset to Default" to restore the original background

Language Switching
Click the settings icon (⚙️) in the bottom right

Go to "Appearance" tab

Select your preferred language from the dropdown menu

The interface will update immediately without refresh

🔧 Development
Project Structure
text
GenresFox/
├── src/
│   ├── _locales/           # Internationalization files
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # Extension icon
│   ├── manifest.json       # Extension manifest
│   ├── newtab.html         # Main HTML file
│   ├── script.js           # Main JavaScript logic
│   ├── search.js           # Search bar & search button logic
│   ├── i18n.js             # Internationalization module
│   ├── wallpaper.js        # Wallpaper management module
│   ├── accessibility.js    # Accessibility features module
│   ├── image-processor.js  # High-performance image processing module
│   ├── image-worker.js     # Web Worker for background image processing
│   ├── styles.css          # Main styles
│   ├── search.css          # Search bar styles
│   └── accessibility.css   # Accessibility styles
├── CHANGELOG.md
└── README.md
Technologies Used
Manifest V3: Latest Chrome extension standard

Vanilla JavaScript: No frameworks, pure performance

CSS3: Modern styling with glassmorphism effects

Web Workers: Background image processing without blocking UI

IndexedDB: For storing large wallpaper files and cache

LocalStorage: For persistent settings and metadata caching

Chrome Extension APIs: For internationalization and browser integration

Adding New Languages
Create a new folder in src/_locales/ with the language code (e.g., fr for French)

Copy messages.json from en folder

Translate all message values

Add the language to _fallbackMessages in src/i18n.js

Update _supportedLanguages array and _detectLanguage() function

Add a language switch entry in the settings UI

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

Fork the project

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

👤 Author
zayoka

GitHub: @zayoka

🙏 Acknowledgments
Inspired by modern web design trends

Icons from Google Material Design

Favicon service by DuckDuckGo (primary) and Google s2 (fallback)

Daily wallpapers by Bing

中文
✨ 功能特性
🎨 现代深色主题: 精美的玻璃态设计，流畅的动画效果

🔍 多引擎搜索: 内置支持 Google、Bing 和 DuckDuckGo

⚙️ 自定义搜索引擎: 使用自定义 URL 添加您自己的搜索引擎

🔖 快速快捷方式: 创建指向您喜爱的网站的快捷方式，自动获取网站图标

🖼️ 自定义壁纸: 上传您自己的背景图片（最大 50MB，50MP），支持拖放上传

🌅 Bing 每日壁纸: 来自 Bing 的美丽每日壁纸，智能 24 小时缓存和预加载

⚡ 高性能图像处理: Web Worker 支持，渐进式预览和智能压缩

🌍 多语言支持: 英语、简体中文、繁体中文、日语、西班牙语、法语、韩语

♿ 无障碍功能: 高对比度主题，字体控制，动画设置，键盘快捷键

⌨️ 键盘快捷键: 快速切换搜索引擎 (Alt+↑↓)，聚焦搜索框 (/)，打开设置 (Alt+,)

💾 智能缓存: 图标缓存、壁纸缓存和处理结果缓存，实现更快加载

🎯 简洁极简: 无干扰界面，专注于重要内容

🌐 语言切换: 通过设置轻松切换语言，支持自动检测

🚀 安装
从源代码安装
克隆此仓库：

bash
git clone https://github.com/zayokami/GenresFox.git
打开 Chrome/Edge 并导航至 chrome://extensions/

在右上角启用"开发者模式"

点击"加载已解压的扩展程序"并选择 src 文件夹

享受您的新标签页！

从 Chrome 网上应用店安装
即将推出...

🛠️ 使用方法
搜索
只需在搜索框中输入并按下 Enter 键

点击搜索引擎图标在不同引擎间切换

URL 会自动检测并直接打开

自定义搜索引擎
点击右下角的设置图标 (⚙️)

转到"搜索和快捷方式"标签页

输入引擎名称和 URL（使用 %s 作为搜索查询占位符）

示例：https://kagi.com/search?q=%s

点击"添加"

快捷方式
打开设置并转到"搜索和快捷方式"标签页

滚动到"快捷方式"部分

输入您喜爱的网站名称和 URL

网站图标将自动获取

自定义壁纸
打开设置并转到"壁纸"标签页

拖放图像或点击上传

最大文件大小：50MB，最大分辨率：5000 万像素

图像会自动优化和压缩以提高存储效率

点击"重置为默认"可恢复原始背景

语言切换
点击右下角的设置图标 (⚙️)

转到"外观"标签页

从下拉菜单中选择您偏好的语言

界面将立即更新，无需刷新

🔧 开发
项目结构
text
GenresFox/
├── src/
│   ├── _locales/           # 国际化文件
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # 扩展图标
│   ├── manifest.json       # 扩展清单
│   ├── newtab.html         # 主 HTML 文件
│   ├── script.js           # 主 JavaScript 逻辑
│   ├── search.js           # 搜索栏和搜索按钮逻辑
│   ├── i18n.js             # 国际化模块
│   ├── wallpaper.js        # 壁纸管理模块
│   ├── accessibility.js    # 无障碍功能模块
│   ├── image-processor.js  # 高性能图像处理模块
│   ├── image-worker.js     # 后台图像处理的 Web Worker
│   ├── styles.css          # 主样式
│   ├── search.css          # 搜索栏样式
│   └── accessibility.css   # 无障碍功能样式
├── CHANGELOG.md
└── README.md
使用的技术
Manifest V3: 最新的 Chrome 扩展标准

Vanilla JavaScript: 无框架，纯性能

CSS3: 现代样式设计，带有玻璃态效果

Web Workers: 后台图像处理，不阻塞 UI

IndexedDB: 用于存储大型壁纸文件和缓存

LocalStorage: 用于持久化设置和元数据缓存

Chrome Extension APIs: 用于国际化和浏览器集成

添加新语言
在 src/_locales/ 中创建以语言代码命名的新文件夹（例如，法语的 fr）

从 en 文件夹复制 messages.json

翻译所有消息值

在 src/i18n.js 的 _fallbackMessages 中添加该语言

更新 _supportedLanguages 数组和 _detectLanguage() 函数

在设置 UI 中添加语言切换条目

🤝 贡献
欢迎贡献！请随时提交 Pull Request。

Fork 项目

创建您的功能分支 (git checkout -b feature/AmazingFeature)

提交您的更改 (git commit -m 'Add some AmazingFeature')

推送到分支 (git push origin feature/AmazingFeature)

打开一个 Pull Request

📝 许可证
本项目采用 MIT 许可证 - 详情请参阅 LICENSE 文件。

👤 作者
zayoka

GitHub: @zayoka

🙏 致谢
灵感来自现代网页设计趋势

图标来自 Google Material Design

网站图标服务由 DuckDuckGo（主要）和 Google s2（备用）提供

每日壁纸由 Bing 提供

日本語
✨ 特徴
🎨 モダンなダークテーマ: 美しいグラスモーフィズムデザインとスムーズなアニメーション

🔍 マルチエンジン検索: Google、Bing、DuckDuckGo の組み込みサポート

⚙️ カスタム検索エンジン: カスタムURLで独自の検索エンジンを追加

🔖 クイックショートカット: お気に入りのウェブサイトへのショートカット作成、ファビコン自動取得

🖼️ カスタム壁紙: 独自の背景画像をアップロード（最大50MB、50MP）、ドラッグ＆ドロップ対応

🌅 Bing デイリー壁紙: Bingからの美しい日替わり壁紙、スマートな24時間キャッシュとプリロード

⚡ 高性能画像処理: Web Workerサポート、プログレッシブプレビュー、インテリジェント圧縮

🌍 多言語対応: 英語、簡体字中国語、繁体字中国語、日本語、スペイン語、フランス語、韓国語

♿ アクセシビリティ: 高コントラストテーマ、フォント制御、アニメーション設定、キーボードショートカット

⌨️ キーボードショートカット: エンジン切り替え (Alt+↑↓)、検索にフォーカス (/)、設定を開く (Alt+,)

💾 スマートキャッシュ: アイコンキャッシュ、壁紙キャッシュ、処理結果キャッシュによる高速読み込み

🎯 クリーンでミニマル: 重要なことに集中できるディストラクションフリーインターフェース

🌐 言語切替: 設定からの簡単な言語切替、自動検出対応

🚀 インストール
ソースからインストール
リポジトリをクローン:

bash
git clone https://github.com/zayokami/GenresFox.git
Chrome/Edgeを開き、chrome://extensions/ に移動

右上の「開発者モード」を有効化

「パッケージ化されていない拡張機能を読み込む」をクリックし、src フォルダを選択

新しいタブページをお楽しみください！

Chrome ウェブストアから
近日公開予定...

🛠️ 使用方法
検索
検索ボックスに入力して Enter キーを押すだけ

検索エンジンアイコンをクリックして異なるエンジン間で切り替え

URLは自動検出され、直接開かれます

カスタム検索エンジン
右下の設定アイコン (⚙️) をクリック

「検索とショートカット」タブに移動

エンジン名とURLを入力（%s を検索クエリのプレースホルダーとして使用）

例: https://kagi.com/search?q=%s

「追加」をクリック

ショートカット
設定を開き、「検索とショートカット」タブに移動

「ショートカット」セクションまでスクロール

お気に入りのウェブサイトの名前とURLを入力

ファビコンが自動的に取得されます

カスタム壁紙
設定を開き、「壁紙」タブに移動

画像をドラッグ＆ドロップまたはクリックしてアップロード

最大ファイルサイズ: 50MB、最大解像度: 5000万ピクセル

画像は自動的に最適化・圧縮され、ストレージ効率が向上

「デフォルトに戻す」をクリックして元の背景を復元

言語切替
右下の設定アイコン (⚙️) をクリック

「外観」タブに移動

ドロップダウンメニューから希望の言語を選択

インターフェースはリフレッシュなしですぐに更新されます

🔧 開発
プロジェクト構造
text
GenresFox/
├── src/
│   ├── _locales/           # 国際化ファイル
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # 拡張機能アイコン
│   ├── manifest.json       # 拡張機能マニフェスト
│   ├── newtab.html         # メインHTMLファイル
│   ├── script.js           # メインJavaScriptロジック
│   ├── search.js           # 検索バーと検索ボタンロジック
│   ├── i18n.js             # 国際化モジュール
│   ├── wallpaper.js        # 壁紙管理モジュール
│   ├── accessibility.js    # アクセシビリティ機能モジュール
│   ├── image-processor.js  # 高性能画像処理モジュール
│   ├── image-worker.js     # バックグラウンド画像処理用Web Worker
│   ├── styles.css          # メインスタイル
│   ├── search.css          # 検索バースタイル
│   └── accessibility.css   # アクセシビリティスタイル
├── CHANGELOG.md
└── README.md
使用技術
Manifest V3: 最新のChrome拡張機能標準

Vanilla JavaScript: フレームワーク不使用、純粋なパフォーマンス

CSS3: グラスモーフィズム効果を備えたモダンスタイリング

Web Workers: UIをブロックしないバックグラウンド画像処理

IndexedDB: 大きな壁紙ファイルとキャッシュの保存用

LocalStorage: 永続的設定とメタデータキャッシュ用

Chrome Extension APIs: 国際化とブラウザ統合用

新しい言語の追加
src/_locales/ に言語コードで新しいフォルダを作成（例: フランス語なら fr）

en フォルダから messages.json をコピー

すべてのメッセージ値を翻訳

src/i18n.js の _fallbackMessages に言語を追加

_supportedLanguages 配列と _detectLanguage() 関数を更新

設定UIに言語切替エントリを追加

🤝 貢献
貢献を歓迎します！ぜひプルリクエストを提出してください。

プロジェクトをフォーク

機能ブランチを作成 (git checkout -b feature/AmazingFeature)

変更をコミット (git commit -m 'Add some AmazingFeature')

ブランチにプッシュ (git push origin feature/AmazingFeature)

プルリクエストを開く

📝 ライセンス
このプロジェクトはMITライセンスの下でライセンスされています - 詳細は LICENSE ファイルを参照してください。

👤 作者
zayoka

GitHub: @zayoka

🙏 謝辞
モダンなWebデザイントレンドに触発

アイコンはGoogle Material Designから

ファビコンサービスはDuckDuckGo（主要）とGoogle s2（代替）

日替わり壁紙はBingから

한국어
✨ 기능
🎨 모던 다크 테마: 아름다운 글래스모피즘 디자인과 부드러운 애니메이션

🔍 멀티 엔진 검색: Google, Bing, DuckDuckGo 내장 지원

⚙️ 커스텀 검색 엔진: 사용자 정의 URL로 자신만의 검색 엔진 추가

🔖 빠른 바로가기: 자동 파비콘 가져오기로 즐겨찾는 웹사이트 바로가기 생성

🖼️ 커스텀 배경화면: 자신의 배경 이미지 업로드 (최대 50MB, 50MP), 드래그 앤 드롭 지원

🌅 Bing 데일리 배경화면: Bing의 아름다운 일일 배경화면, 스마트 24시간 캐싱 및 프리로딩

⚡ 고성능 이미지 처리: Web Worker 지원, 점진적 미리보기, 지능형 압축

🌍 다국어 지원: 영어, 간체 중국어, 번체 중국어, 일본어, 스페인어, 프랑스어, 한국어

♿ 접근성: 고대비 테마, 글꼴 제어, 애니메이션 설정, 키보드 단축키

⌨️ 키보드 단축키: 빠른 엔진 전환 (Alt+↑↓), 검색에 포커스 (/), 설정 열기 (Alt+,)

💾 스마트 캐싱: 아이콘 캐싱, 배경화면 캐싱, 처리 결과 캐싱으로 빠른 로딩

🎯 깔끔하고 미니멀: 중요한 것에 집중할 수 있는 방해 없는 인터페이스

🌐 언어 전환: 설정을 통한 쉬운 언어 전환, 자동 감지 지원

🚀 설치
소스에서 설치
저장소 클론:

bash
git clone https://github.com/zayokami/GenresFox.git
Chrome/Edge를 열고 chrome://extensions/로 이동

오른쪽 상단의 "개발자 모드" 활성화

"압축해제된 확장 프로그램을 로드합니다" 클릭하고 src 폴더 선택

새 탭 페이지를 즐기세요!

Chrome 웹 스토어에서
곧 출시 예정...

🛠️ 사용 방법
검색
검색 상자에 입력하고 Enter 키 누르기만 하면 됩니다

검색 엔진 아이콘을 클릭하여 다른 엔진 간 전환

URL은 자동으로 감지되어 직접 열립니다

커스텀 검색 엔진
오른쪽 하단 설정 아이콘 (⚙️) 클릭

"검색 및 바로가기" 탭으로 이동

엔진 이름과 URL 입력 (검색 쿼리 자리 표시자로 %s 사용)

예: https://kagi.com/search?q=%s

"추가" 클릭

바로가기
설정 열고 "검색 및 바로가기" 탭으로 이동

"바로가기" 섹션으로 스크롤

즐겨찾는 웹사이트의 이름과 URL 입력

파비콘이 자동으로 가져와집니다

커스텀 배경화면
설정 열고 "배경화면" 탭으로 이동

이미지 드래그 앤 드롭 또는 클릭하여 업로드

최대 파일 크기: 50MB, 최대 해상도: 5000만 화소

이미지는 자동으로 최적화 및 압축되어 저장 효율성 향상

"기본값으로 재설정" 클릭하여 원래 배경 복원

언어 전환
오른쪽 하단 설정 아이콘 (⚙️) 클릭

"외관" 탭으로 이동

드롭다운 메뉴에서 선호하는 언어 선택

인터페이스는 새로고침 없이 즉시 업데이트됩니다

🔧 개발
프로젝트 구조
text
GenresFox/
├── src/
│   ├── _locales/           # 국제화 파일
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # 확장 프로그램 아이콘
│   ├── manifest.json       # 확장 프로그램 매니페스트
│   ├── newtab.html         # 메인 HTML 파일
│   ├── script.js           # 메인 JavaScript 로직
│   ├── search.js           # 검색창 및 검색 버튼 로직
│   ├── i18n.js             # 국제화 모듈
│   ├── wallpaper.js        # 배경화면 관리 모듈
│   ├── accessibility.js    # 접근성 기능 모듈
│   ├── image-processor.js  # 고성능 이미지 처리 모듈
│   ├── image-worker.js     # 배경 이미지 처리용 Web Worker
│   ├── styles.css          # 메인 스타일
│   ├── search.css          # 검색창 스타일
│   └── accessibility.css   # 접근성 스타일
├── CHANGELOG.md
└── README.md
사용 기술
Manifest V3: 최신 Chrome 확장 프로그램 표준

Vanilla JavaScript: 프레임워크 없음, 순수 성능

CSS3: 글래스모피즘 효과가 있는 모던 스타일링

Web Workers: UI 차단 없는 배경 이미지 처리

IndexedDB: 대용량 배경화면 파일 및 캐시 저장용

LocalStorage: 영구 설정 및 메타데이터 캐싱용

Chrome Extension APIs: 국제화 및 브라우저 통합용

새 언어 추가
src/_locales/에 언어 코드로 새 폴더 생성 (예: 프랑스어는 fr)

en 폴더에서 messages.json 복사

모든 메시지 값 번역

src/i18n.js의 _fallbackMessages에 언어 추가

_supportedLanguages 배열 및 _detectLanguage() 함수 업데이트

설정 UI에 언어 전환 항목 추가

🤝 기여
기여를 환영합니다! 풀 리퀘스트를 자유롭게 제출해 주세요.

프로젝트 포크

기능 브랜치 생성 (git checkout -b feature/AmazingFeature)

변경 사항 커밋 (git commit -m 'Add some AmazingFeature')

브랜치에 푸시 (git push origin feature/AmazingFeature)

풀 리퀘스트 열기

📝 라이선스
이 프로젝트는 MIT 라이선스 하에 라이선스가 부여됩니다 - 자세한 내용은 LICENSE 파일을 참조하세요.

👤 저자
zayoka

GitHub: @zayoka

🙏 감사의 말
현대 웹 디자인 트렌드에서 영감

아이콘은 Google Material Design에서

파비콘 서비스는 DuckDuckGo (주) 및 Google s2 (대체)

일일 배경화면은 Bing에서 제공

Español
✨ Características
🎨 Tema Oscuro Moderno: Hermoso diseño de glassmorphism con animaciones suaves

🔍 Búsqueda Multi-Motor: Soporte incorporado para Google, Bing y DuckDuckGo

⚙️ Motores de Búsqueda Personalizados: Agrega tus propios motores de búsqueda con URLs personalizadas

🔖 Accesos Directos Rápidos: Crea accesos directos a tus sitios web favoritos con favicons obtenidos automáticamente

🖼️ Fondos de Pantalla Personalizados: Sube tus propias imágenes de fondo (hasta 50MB, 50MP) con soporte de arrastrar y soltar

🌅 Fondo de Pantalla Diario de Bing: Hermosos fondos de pantalla diarios de Bing con caché inteligente de 24 horas y precarga

⚡ Procesamiento de Imágenes de Alto Rendimiento: Soporte para Web Worker, vista previa progresiva y compresión inteligente

🌍 Multi-idioma: Inglés, Chino Simplificado, Chino Tradicional, Japonés, Español, Francés, Coreano

♿ Accesibilidad: Temas de alto contraste, controles de fuente, configuraciones de animación, atajos de teclado

⌨️ Atajos de Teclado: Cambio rápido de motor (Alt+↑↓), enfoque en búsqueda (/), abrir configuración (Alt+,)

💾 Caché Inteligente: Caché de iconos, caché de fondos de pantalla y caché de resultados de procesamiento para carga más rápida

🎯 Limpio y Mínimo: Interfaz sin distracciones centrada en lo importante

🌐 Cambio de Idioma: Cambio fácil de idioma a través de configuración con detección automática

🚀 Instalación
Desde el Código Fuente
Clona este repositorio:

bash
git clone https://github.com/zayokami/GenresFox.git
Abre Chrome/Edge y navega a chrome://extensions/

Habilita el "Modo desarrollador" en la esquina superior derecha

Haz clic en "Cargar extensión descomprimida" y selecciona la carpeta src

¡Disfruta de tu nueva página de pestaña!

Desde Chrome Web Store
Próximamente...

🛠️ Uso
Búsqueda
Simplemente escribe en el cuadro de búsqueda y presiona Enter

Haz clic en el icono del motor de búsqueda para cambiar entre diferentes motores

Las URLs se detectan automáticamente y se abren directamente

Motores de Búsqueda Personalizados
Haz clic en el icono de configuración (⚙️) en la esquina inferior derecha

Ve a la pestaña "Búsqueda y Accesos Directos"

Ingresa el nombre del motor y la URL (usa %s como marcador de posición de consulta de búsqueda)

Ejemplo: https://kagi.com/search?q=%s

Haz clic en "Agregar"

Accesos Directos
Abre configuración y ve a la pestaña "Búsqueda y Accesos Directos"

Desplázate a la sección "Accesos Directos"

Ingresa el nombre y la URL de tu sitio web favorito

El favicon se obtendrá automáticamente

Fondo de Pantalla Personalizado
Abre configuración y ve a la pestaña "Fondo de Pantalla"

Arrastra y suelta una imagen o haz clic para subir

Tamaño máximo de archivo: 50MB, resolución máxima: 50 megapíxeles

Las imágenes se optimizan y comprimen automáticamente para mayor eficiencia de almacenamiento

Haz clic en "Restablecer a Predeterminado" para restaurar el fondo original

Cambio de Idioma
Haz clic en el icono de configuración (⚙️) en la esquina inferior derecha

Ve a la pestaña "Apariencia"

Selecciona tu idioma preferido del menú desplegable

La interfaz se actualizará inmediatamente sin necesidad de actualizar

🔧 Desarrollo
Estructura del Proyecto
text
GenresFox/
├── src/
│   ├── _locales/           # Archivos de internacionalización
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # Icono de extensión
│   ├── manifest.json       # Manifiesto de extensión
│   ├── newtab.html         # Archivo HTML principal
│   ├── script.js           # Lógica principal de JavaScript
│   ├── search.js           # Lógica de barra de búsqueda y botones
│   ├── i18n.js             # Módulo de internacionalización
│   ├── wallpaper.js        # Módulo de gestión de fondos de pantalla
│   ├── accessibility.js    # Módulo de funciones de accesibilidad
│   ├── image-processor.js  # Módulo de procesamiento de imágenes de alto rendimiento
│   ├── image-worker.js     # Web Worker para procesamiento de imágenes en segundo plano
│   ├── styles.css          # Estilos principales
│   ├── search.css          # Estilos de barra de búsqueda
│   └── accessibility.css   # Estilos de accesibilidad
├── CHANGELOG.md
└── README.md
Tecnologías Utilizadas
Manifest V3: Estándar más reciente de extensiones de Chrome

Vanilla JavaScript: Sin frameworks, rendimiento puro

CSS3: Estilizado moderno con efectos de glassmorphism

Web Workers: Procesamiento de imágenes en segundo plano sin bloquear la UI

IndexedDB: Para almacenar archivos grandes de fondos de pantalla y caché

LocalStorage: Para configuraciones persistentes y caché de metadatos

Chrome Extension APIs: Para internacionalización e integración del navegador

Agregar Nuevos Idiomas
Crea una nueva carpeta en src/_locales/ con el código de idioma (ej., fr para francés)

Copia messages.json de la carpeta en

Traduce todos los valores de mensaje

Agrega el idioma a _fallbackMessages en src/i18n.js

Actualiza el arreglo _supportedLanguages y la función _detectLanguage()

Agrega una entrada de cambio de idioma en la UI de configuración

🤝 Contribuciones
¡Las contribuciones son bienvenidas! No dudes en enviar un Pull Request.

Haz un fork del proyecto

Crea tu rama de funcionalidad (git checkout -b feature/AmazingFeature)

Confirma tus cambios (git commit -m 'Add some AmazingFeature')

Sube a la rama (git push origin feature/AmazingFeature)

Abre un Pull Request

📝 Licencia
Este proyecto está bajo la Licencia MIT - consulta el archivo LICENSE para más detalles.

👤 Autor
zayoka

GitHub: @zayoka

🙏 Agradecimientos
Inspirado por tendencias modernas de diseño web

Iconos de Google Material Design

Servicio de favicon por DuckDuckGo (principal) y Google s2 (alternativa)

Fondos de pantalla diarios por Bing

Français
✨ Fonctionnalités
🎨 Thème Sombre Moderne: Beau design glassmorphism avec des animations fluides

🔍 Recherche Multi-Moteurs: Prise en charge intégrée de Google, Bing et DuckDuckGo

⚙️ Moteurs de Recherche Personnalisés: Ajoutez vos propres moteurs de recherche avec des URLs personnalisées

🔖 Raccourcis Rapides: Créez des raccourcis vers vos sites web préférés avec favicons récupérés automatiquement

🖼️ Fond d'Écran Personnalisé: Téléchargez vos propres images de fond (jusqu'à 50MB, 50MP) avec prise en charge du glisser-déposer

🌅 Fond d'Écran Quotidien Bing: De beaux fonds d'écran quotidiens de Bing avec mise en cache intelligente de 24 heures et préchargement

⚡ Traitement d'Image Haute Performance: Prise en charge des Web Workers, prévisualisation progressive et compression intelligente

🌍 Multi-langue: Anglais, Chinois Simplifié, Chinois Traditionnel, Japonais, Espagnol, Français, Coréen

♿ Accessibilité: Thèmes à haut contraste, contrôles de police, paramètres d'animation, raccourcis clavier

⌨️ Raccourcis Clavier: Changement rapide de moteur (Alt+↑↓), focus sur la recherche (/), ouvrir les paramètres (Alt+,)

💾 Mise en Cache Intelligente: Mise en cache d'icônes, de fonds d'écran et de résultats de traitement pour un chargement plus rapide

🎯 Propre et Minimal: Interface sans distraction axée sur l'essentiel

🌐 Changement de Langue: Changement facile de langue via les paramètres avec détection automatique

🚀 Installation
À partir du Code Source
Clonez ce dépôt :

bash
git clone https://github.com/zayokami/GenresFox.git
Ouvrez Chrome/Edge et naviguez vers chrome://extensions/

Activez le "Mode développeur" dans le coin supérieur droit

Cliquez sur "Charger l'extension non empaquetée" et sélectionnez le dossier src

Profitez de votre nouvelle page d'onglet !

Depuis le Chrome Web Store
Bientôt disponible...

🛠️ Utilisation
Recherche
Tapez simplement dans la zone de recherche et appuyez sur Entrée

Cliquez sur l'icône du moteur de recherche pour basculer entre différents moteurs

Les URLs sont automatiquement détectées et ouvertes directement

Moteurs de Recherche Personnalisés
Cliquez sur l'icône des paramètres (⚙️) en bas à droite

Allez dans l'onglet "Recherche et Raccourcis"

Entrez le nom du moteur et l'URL (utilisez %s comme espace réservé pour la requête de recherche)

Exemple : https://kagi.com/search?q=%s

Cliquez sur "Ajouter"

Raccourcis
Ouvrez les paramètres et allez dans l'onglet "Recherche et Raccourcis"

Faites défiler jusqu'à la section "Raccourcis"

Entrez le nom et l'URL de votre site web préféré

Le favicon sera récupéré automatiquement

Fond d'Écran Personnalisé
Ouvrez les paramètres et allez dans l'onglet "Fond d'écran"

Glissez-déposez une image ou cliquez pour télécharger

Taille maximale du fichier : 50MB, résolution maximale : 50 mégapixels

Les images sont automatiquement optimisées et compressées pour une efficacité de stockage

Cliquez sur "Rétablir la valeur par défaut" pour restaurer l'arrière-plan d'origine

Changement de Langue
Cliquez sur l'icône des paramètres (⚙️) en bas à droite

Allez dans l'onglet "Apparence"

Sélectionnez votre langue préférée dans le menu déroulant

L'interface sera mise à jour immédiatement sans actualisation

🔧 Développement
Structure du Projet
text
GenresFox/
├── src/
│   ├── _locales/           # Fichiers d'internationalisation
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # Icône de l'extension
│   ├── manifest.json       # Manifeste de l'extension
│   ├── newtab.html         # Fichier HTML principal
│   ├── script.js           # Logique JavaScript principale
│   ├── search.js           # Logique de la barre de recherche et des boutons
│   ├── i18n.js             # Module d'internationalisation
│   ├── wallpaper.js        # Module de gestion des fonds d'écran
│   ├── accessibility.js    # Module de fonctionnalités d'accessibilité
│   ├── image-processor.js  # Module de traitement d'image haute performance
│   ├── image-worker.js     # Web Worker pour le traitement d'image en arrière-plan
│   ├── styles.css          # Styles principaux
│   ├── search.css          # Styles de la barre de recherche
│   └── accessibility.css   # Styles d'accessibilité
├── CHANGELOG.md
└── README.md
Technologies Utilisées
Manifest V3: Dernière norme d'extension Chrome

Vanilla JavaScript: Sans frameworks, performances pures

CSS3: Style moderne avec effets glassmorphism

Web Workers: Traitement d'image en arrière-plan sans bloquer l'interface utilisateur

IndexedDB: Pour stocker les fichiers de fond d'écran volumineux et le cache

LocalStorage: Pour les paramètres persistants et la mise en cache des métadonnées

Chrome Extension APIs: Pour l'internationalisation et l'intégration du navigateur

Ajouter de Nouvelles Langues
Créez un nouveau dossier dans src/_locales/ avec le code de langue (ex. fr pour le français)

Copiez messages.json depuis le dossier en

Traduisez toutes les valeurs de messages

Ajoutez la langue à _fallbackMessages dans src/i18n.js

Mettez à jour le tableau _supportedLanguages et la fonction _detectLanguage()

Ajoutez une entrée de changement de langue dans l'interface utilisateur des paramètres

🤝 Contributions
Les contributions sont les bienvenues ! N'hésitez pas à soumettre une Pull Request.

Forkez le projet

Créez votre branche de fonctionnalité (git checkout -b feature/AmazingFeature)

Committez vos modifications (git commit -m 'Add some AmazingFeature')

Poussez vers la branche (git push origin feature/AmazingFeature)

Ouvrez une Pull Request

📝 Licence
Ce projet est sous licence MIT - voir le fichier LICENSE pour plus de détails.

👤 Auteur
zayoka

GitHub : @zayoka

🙏 Remerciements
Inspiré par les tendances modernes de conception web

Icônes de Google Material Design

Service de favicon par DuckDuckGo (principal) et Google s2 (alternative)

Fonds d'écran quotidiens par Bing

GenresFox
<div align="center">
https://img.shields.io/badge/version-0.3.8-blue.svg
https://img.shields.io/badge/license-MIT-green.svg
https://img.shields.io/badge/chrome-manifest%2520v3-orange.svg

完全开源、极其简洁、高度可定制的新标签页扩展

English | 中文 | 日本語 | 한국어 | Español | Français

https://assets/Screenshots/Show-1.png

</div>
English
✨ Features
🎨 Modern Dark Theme: Beautiful glassmorphism design with smooth animations

🔍 Multi-Engine Search: Built-in support for Google, Bing, and DuckDuckGo

⚙️ Custom Search Engines: Add your own search engines with custom URLs

🔖 Quick Shortcuts: Create shortcuts to your favorite websites with auto-fetched favicons

🖼️ Custom Wallpapers: Upload your own background images (up to 50MB, 50MP) with drag-and-drop support

🌅 Bing Daily Wallpaper: Beautiful daily wallpapers from Bing with smart 24-hour caching and preloading

⚡ High-Performance Image Processing: Web Worker support, progressive preview, and intelligent compression

🌍 Multi-language: English, Simplified Chinese, Traditional Chinese, Japanese, Spanish, French, Korean

♿ Accessibility: High contrast themes, font controls, animation settings, keyboard shortcuts

⌨️ Keyboard Shortcuts: Quick engine switching (Alt+↑↓), focus search (/), open settings (Alt+,)

💾 Smart Caching: Icon caching, wallpaper caching, and processing result caching for faster loading

🎯 Clean & Minimal: Distraction-free interface focused on what matters

🌐 Language Switching: Easy language switching through settings with auto-detection

🚀 Installation
From Source
Clone this repository:

bash
git clone https://github.com/zayokami/GenresFox.git
Open Chrome/Edge and navigate to chrome://extensions/

Enable "Developer mode" in the top right corner

Click "Load unpacked" and select the src folder

Enjoy your new tab page!

From Chrome Web Store
Coming soon...

🛠️ Usage
Search
Simply type in the search box and press Enter

Click the search engine icon to switch between different engines

URLs are automatically detected and opened directly

Custom Search Engines
Click the settings icon (⚙️) in the bottom right

Go to "Search & Shortcuts" tab

Enter the engine name and URL (use %s as the search query placeholder)

Example: https://kagi.com/search?q=%s

Click "Add"

Shortcuts
Open settings and go to "Search & Shortcuts" tab

Scroll to the "Shortcuts" section

Enter the name and URL of your favorite website

The favicon will be automatically fetched

Custom Wallpaper
Open settings and go to "Wallpaper" tab

Drag and drop an image or click to upload

Maximum file size: 50MB, maximum resolution: 50 megapixels

Images are automatically optimized and compressed for storage efficiency

Click "Reset to Default" to restore the original background

Language Switching
Click the settings icon (⚙️) in the bottom right

Go to "Appearance" tab

Select your preferred language from the dropdown menu

The interface will update immediately without refresh

🔧 Development
Project Structure
text
GenresFox/
├── src/
│   ├── _locales/           # Internationalization files
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # Extension icon
│   ├── manifest.json       # Extension manifest
│   ├── newtab.html         # Main HTML file
│   ├── script.js           # Main JavaScript logic
│   ├── search.js           # Search bar & search button logic
│   ├── i18n.js             # Internationalization module
│   ├── wallpaper.js        # Wallpaper management module
│   ├── accessibility.js    # Accessibility features module
│   ├── image-processor.js  # High-performance image processing module
│   ├── image-worker.js     # Web Worker for background image processing
│   ├── styles.css          # Main styles
│   ├── search.css          # Search bar styles
│   └── accessibility.css   # Accessibility styles
├── CHANGELOG.md
└── README.md
Technologies Used
Manifest V3: Latest Chrome extension standard

Vanilla JavaScript: No frameworks, pure performance

CSS3: Modern styling with glassmorphism effects

Web Workers: Background image processing without blocking UI

IndexedDB: For storing large wallpaper files and cache

LocalStorage: For persistent settings and metadata caching

Chrome Extension APIs: For internationalization and browser integration

Adding New Languages
Create a new folder in src/_locales/ with the language code (e.g., fr for French)

Copy messages.json from en folder

Translate all message values

Add the language to _fallbackMessages in src/i18n.js

Update _supportedLanguages array and _detectLanguage() function

Add a language switch entry in the settings UI

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

Fork the project

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

👤 Author
zayoka

GitHub: @zayoka

🙏 Acknowledgments
Inspired by modern web design trends

Icons from Google Material Design

Favicon service by DuckDuckGo (primary) and Google s2 (fallback)

Daily wallpapers by Bing

中文
✨ 功能特性
🎨 现代深色主题: 精美的玻璃态设计，流畅的动画效果

🔍 多引擎搜索: 内置支持 Google、Bing 和 DuckDuckGo

⚙️ 自定义搜索引擎: 使用自定义 URL 添加您自己的搜索引擎

🔖 快速快捷方式: 创建指向您喜爱的网站的快捷方式，自动获取网站图标

🖼️ 自定义壁纸: 上传您自己的背景图片（最大 50MB，50MP），支持拖放上传

🌅 Bing 每日壁纸: 来自 Bing 的美丽每日壁纸，智能 24 小时缓存和预加载

⚡ 高性能图像处理: Web Worker 支持，渐进式预览和智能压缩

🌍 多语言支持: 英语、简体中文、繁体中文、日语、西班牙语、法语、韩语

♿ 无障碍功能: 高对比度主题，字体控制，动画设置，键盘快捷键

⌨️ 键盘快捷键: 快速切换搜索引擎 (Alt+↑↓)，聚焦搜索框 (/)，打开设置 (Alt+,)

💾 智能缓存: 图标缓存、壁纸缓存和处理结果缓存，实现更快加载

🎯 简洁极简: 无干扰界面，专注于重要内容

🌐 语言切换: 通过设置轻松切换语言，支持自动检测

🚀 安装
从源代码安装
克隆此仓库：

bash
git clone https://github.com/zayokami/GenresFox.git
打开 Chrome/Edge 并导航至 chrome://extensions/

在右上角启用"开发者模式"

点击"加载已解压的扩展程序"并选择 src 文件夹

享受您的新标签页！

从 Chrome 网上应用店安装
即将推出...

🛠️ 使用方法
搜索
只需在搜索框中输入并按下 Enter 键

点击搜索引擎图标在不同引擎间切换

URL 会自动检测并直接打开

自定义搜索引擎
点击右下角的设置图标 (⚙️)

转到"搜索和快捷方式"标签页

输入引擎名称和 URL（使用 %s 作为搜索查询占位符）

示例：https://kagi.com/search?q=%s

点击"添加"

快捷方式
打开设置并转到"搜索和快捷方式"标签页

滚动到"快捷方式"部分

输入您喜爱的网站名称和 URL

网站图标将自动获取

自定义壁纸
打开设置并转到"壁纸"标签页

拖放图像或点击上传

最大文件大小：50MB，最大分辨率：5000 万像素

图像会自动优化和压缩以提高存储效率

点击"重置为默认"可恢复原始背景

语言切换
点击右下角的设置图标 (⚙️)

转到"外观"标签页

从下拉菜单中选择您偏好的语言

界面将立即更新，无需刷新

🔧 开发
项目结构
text
GenresFox/
├── src/
│   ├── _locales/           # 国际化文件
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # 扩展图标
│   ├── manifest.json       # 扩展清单
│   ├── newtab.html         # 主 HTML 文件
│   ├── script.js           # 主 JavaScript 逻辑
│   ├── search.js           # 搜索栏和搜索按钮逻辑
│   ├── i18n.js             # 国际化模块
│   ├── wallpaper.js        # 壁纸管理模块
│   ├── accessibility.js    # 无障碍功能模块
│   ├── image-processor.js  # 高性能图像处理模块
│   ├── image-worker.js     # 后台图像处理的 Web Worker
│   ├── styles.css          # 主样式
│   ├── search.css          # 搜索栏样式
│   └── accessibility.css   # 无障碍功能样式
├── CHANGELOG.md
└── README.md
使用的技术
Manifest V3: 最新的 Chrome 扩展标准

Vanilla JavaScript: 无框架，纯性能

CSS3: 现代样式设计，带有玻璃态效果

Web Workers: 后台图像处理，不阻塞 UI

IndexedDB: 用于存储大型壁纸文件和缓存

LocalStorage: 用于持久化设置和元数据缓存

Chrome Extension APIs: 用于国际化和浏览器集成

添加新语言
在 src/_locales/ 中创建以语言代码命名的新文件夹（例如，法语的 fr）

从 en 文件夹复制 messages.json

翻译所有消息值

在 src/i18n.js 的 _fallbackMessages 中添加该语言

更新 _supportedLanguages 数组和 _detectLanguage() 函数

在设置 UI 中添加语言切换条目

🤝 贡献
欢迎贡献！请随时提交 Pull Request。

Fork 项目

创建您的功能分支 (git checkout -b feature/AmazingFeature)

提交您的更改 (git commit -m 'Add some AmazingFeature')

推送到分支 (git push origin feature/AmazingFeature)

打开一个 Pull Request

📝 许可证
本项目采用 MIT 许可证 - 详情请参阅 LICENSE 文件。

👤 作者
zayoka

GitHub: @zayoka

🙏 致谢
灵感来自现代网页设计趋势

图标来自 Google Material Design

网站图标服务由 DuckDuckGo（主要）和 Google s2（备用）提供

每日壁纸由 Bing 提供

日本語
✨ 特徴
🎨 モダンなダークテーマ: 美しいグラスモーフィズムデザインとスムーズなアニメーション

🔍 マルチエンジン検索: Google、Bing、DuckDuckGo の組み込みサポート

⚙️ カスタム検索エンジン: カスタムURLで独自の検索エンジンを追加

🔖 クイックショートカット: お気に入りのウェブサイトへのショートカット作成、ファビコン自動取得

🖼️ カスタム壁紙: 独自の背景画像をアップロード（最大50MB、50MP）、ドラッグ＆ドロップ対応

🌅 Bing デイリー壁紙: Bingからの美しい日替わり壁紙、スマートな24時間キャッシュとプリロード

⚡ 高性能画像処理: Web Workerサポート、プログレッシブプレビュー、インテリジェント圧縮

🌍 多言語対応: 英語、簡体字中国語、繁体字中国語、日本語、スペイン語、フランス語、韓国語

♿ アクセシビリティ: 高コントラストテーマ、フォント制御、アニメーション設定、キーボードショートカット

⌨️ キーボードショートカット: エンジン切り替え (Alt+↑↓)、検索にフォーカス (/)、設定を開く (Alt+,)

💾 スマートキャッシュ: アイコンキャッシュ、壁紙キャッシュ、処理結果キャッシュによる高速読み込み

🎯 クリーンでミニマル: 重要なことに集中できるディストラクションフリーインターフェース

🌐 言語切替: 設定からの簡単な言語切替、自動検出対応

🚀 インストール
ソースからインストール
リポジトリをクローン:

bash
git clone https://github.com/zayokami/GenresFox.git
Chrome/Edgeを開き、chrome://extensions/ に移動

右上の「開発者モード」を有効化

「パッケージ化されていない拡張機能を読み込む」をクリックし、src フォルダを選択

新しいタブページをお楽しみください！

Chrome ウェブストアから
近日公開予定...

🛠️ 使用方法
検索
検索ボックスに入力して Enter キーを押すだけ

検索エンジンアイコンをクリックして異なるエンジン間で切り替え

URLは自動検出され、直接開かれます

カスタム検索エンジン
右下の設定アイコン (⚙️) をクリック

「検索とショートカット」タブに移動

エンジン名とURLを入力（%s を検索クエリのプレースホルダーとして使用）

例: https://kagi.com/search?q=%s

「追加」をクリック

ショートカット
設定を開き、「検索とショートカット」タブに移動

「ショートカット」セクションまでスクロール

お気に入りのウェブサイトの名前とURLを入力

ファビコンが自動的に取得されます

カスタム壁紙
設定を開き、「壁紙」タブに移動

画像をドラッグ＆ドロップまたはクリックしてアップロード

最大ファイルサイズ: 50MB、最大解像度: 5000万ピクセル

画像は自動的に最適化・圧縮され、ストレージ効率が向上

「デフォルトに戻す」をクリックして元の背景を復元

言語切替
右下の設定アイコン (⚙️) をクリック

「外観」タブに移動

ドロップダウンメニューから希望の言語を選択

インターフェースはリフレッシュなしですぐに更新されます

🔧 開発
プロジェクト構造
text
GenresFox/
├── src/
│   ├── _locales/           # 国際化ファイル
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # 拡張機能アイコン
│   ├── manifest.json       # 拡張機能マニフェスト
│   ├── newtab.html         # メインHTMLファイル
│   ├── script.js           # メインJavaScriptロジック
│   ├── search.js           # 検索バーと検索ボタンロジック
│   ├── i18n.js             # 国際化モジュール
│   ├── wallpaper.js        # 壁紙管理モジュール
│   ├── accessibility.js    # アクセシビリティ機能モジュール
│   ├── image-processor.js  # 高性能画像処理モジュール
│   ├── image-worker.js     # バックグラウンド画像処理用Web Worker
│   ├── styles.css          # メインスタイル
│   ├── search.css          # 検索バースタイル
│   └── accessibility.css   # アクセシビリティスタイル
├── CHANGELOG.md
└── README.md
使用技術
Manifest V3: 最新のChrome拡張機能標準

Vanilla JavaScript: フレームワーク不使用、純粋なパフォーマンス

CSS3: グラスモーフィズム効果を備えたモダンスタイリング

Web Workers: UIをブロックしないバックグラウンド画像処理

IndexedDB: 大きな壁紙ファイルとキャッシュの保存用

LocalStorage: 永続的設定とメタデータキャッシュ用

Chrome Extension APIs: 国際化とブラウザ統合用

新しい言語の追加
src/_locales/ に言語コードで新しいフォルダを作成（例: フランス語なら fr）

en フォルダから messages.json をコピー

すべてのメッセージ値を翻訳

src/i18n.js の _fallbackMessages に言語を追加

_supportedLanguages 配列と _detectLanguage() 関数を更新

設定UIに言語切替エントリを追加

🤝 貢献
貢献を歓迎します！ぜひプルリクエストを提出してください。

プロジェクトをフォーク

機能ブランチを作成 (git checkout -b feature/AmazingFeature)

変更をコミット (git commit -m 'Add some AmazingFeature')

ブランチにプッシュ (git push origin feature/AmazingFeature)

プルリクエストを開く

📝 ライセンス
このプロジェクトはMITライセンスの下でライセンスされています - 詳細は LICENSE ファイルを参照してください。

👤 作者
zayoka

GitHub: @zayoka

🙏 謝辞
モダンなWebデザイントレンドに触発

アイコンはGoogle Material Designから

ファビコンサービスはDuckDuckGo（主要）とGoogle s2（代替）

日替わり壁紙はBingから

한국어
✨ 기능
🎨 모던 다크 테마: 아름다운 글래스모피즘 디자인과 부드러운 애니메이션

🔍 멀티 엔진 검색: Google, Bing, DuckDuckGo 내장 지원

⚙️ 커스텀 검색 엔진: 사용자 정의 URL로 자신만의 검색 엔진 추가

🔖 빠른 바로가기: 자동 파비콘 가져오기로 즐겨찾는 웹사이트 바로가기 생성

🖼️ 커스텀 배경화면: 자신의 배경 이미지 업로드 (최대 50MB, 50MP), 드래그 앤 드롭 지원

🌅 Bing 데일리 배경화면: Bing의 아름다운 일일 배경화면, 스마트 24시간 캐싱 및 프리로딩

⚡ 고성능 이미지 처리: Web Worker 지원, 점진적 미리보기, 지능형 압축

🌍 다국어 지원: 영어, 간체 중국어, 번체 중국어, 일본어, 스페인어, 프랑스어, 한국어

♿ 접근성: 고대비 테마, 글꼴 제어, 애니메이션 설정, 키보드 단축키

⌨️ 키보드 단축키: 빠른 엔진 전환 (Alt+↑↓), 검색에 포커스 (/), 설정 열기 (Alt+,)

💾 스마트 캐싱: 아이콘 캐싱, 배경화면 캐싱, 처리 결과 캐싱으로 빠른 로딩

🎯 깔끔하고 미니멀: 중요한 것에 집중할 수 있는 방해 없는 인터페이스

🌐 언어 전환: 설정을 통한 쉬운 언어 전환, 자동 감지 지원

🚀 설치
소스에서 설치
저장소 클론:

bash
git clone https://github.com/zayokami/GenresFox.git
Chrome/Edge를 열고 chrome://extensions/로 이동

오른쪽 상단의 "개발자 모드" 활성화

"압축해제된 확장 프로그램을 로드합니다" 클릭하고 src 폴더 선택

새 탭 페이지를 즐기세요!

Chrome 웹 스토어에서
곧 출시 예정...

🛠️ 사용 방법
검색
검색 상자에 입력하고 Enter 키 누르기만 하면 됩니다

검색 엔진 아이콘을 클릭하여 다른 엔진 간 전환

URL은 자동으로 감지되어 직접 열립니다

커스텀 검색 엔진
오른쪽 하단 설정 아이콘 (⚙️) 클릭

"검색 및 바로가기" 탭으로 이동

엔진 이름과 URL 입력 (검색 쿼리 자리 표시자로 %s 사용)

예: https://kagi.com/search?q=%s

"추가" 클릭

바로가기
설정 열고 "검색 및 바로가기" 탭으로 이동

"바로가기" 섹션으로 스크롤

즐겨찾는 웹사이트의 이름과 URL 입력

파비콘이 자동으로 가져와집니다

커스텀 배경화면
설정 열고 "배경화면" 탭으로 이동

이미지 드래그 앤 드롭 또는 클릭하여 업로드

최대 파일 크기: 50MB, 최대 해상도: 5000만 화소

이미지는 자동으로 최적화 및 압축되어 저장 효율성 향상

"기본값으로 재설정" 클릭하여 원래 배경 복원

언어 전환
오른쪽 하단 설정 아이콘 (⚙️) 클릭

"외관" 탭으로 이동

드롭다운 메뉴에서 선호하는 언어 선택

인터페이스는 새로고침 없이 즉시 업데이트됩니다

🔧 개발
프로젝트 구조
text
GenresFox/
├── src/
│   ├── _locales/           # 국제화 파일
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # 확장 프로그램 아이콘
│   ├── manifest.json       # 확장 프로그램 매니페스트
│   ├── newtab.html         # 메인 HTML 파일
│   ├── script.js           # 메인 JavaScript 로직
│   ├── search.js           # 검색창 및 검색 버튼 로직
│   ├── i18n.js             # 국제화 모듈
│   ├── wallpaper.js        # 배경화면 관리 모듈
│   ├── accessibility.js    # 접근성 기능 모듈
│   ├── image-processor.js  # 고성능 이미지 처리 모듈
│   ├── image-worker.js     # 배경 이미지 처리용 Web Worker
│   ├── styles.css          # 메인 스타일
│   ├── search.css          # 검색창 스타일
│   └── accessibility.css   # 접근성 스타일
├── CHANGELOG.md
└── README.md
사용 기술
Manifest V3: 최신 Chrome 확장 프로그램 표준

Vanilla JavaScript: 프레임워크 없음, 순수 성능

CSS3: 글래스모피즘 효과가 있는 모던 스타일링

Web Workers: UI 차단 없는 배경 이미지 처리

IndexedDB: 대용량 배경화면 파일 및 캐시 저장용

LocalStorage: 영구 설정 및 메타데이터 캐싱용

Chrome Extension APIs: 국제화 및 브라우저 통합용

새 언어 추가
src/_locales/에 언어 코드로 새 폴더 생성 (예: 프랑스어는 fr)

en 폴더에서 messages.json 복사

모든 메시지 값 번역

src/i18n.js의 _fallbackMessages에 언어 추가

_supportedLanguages 배열 및 _detectLanguage() 함수 업데이트

설정 UI에 언어 전환 항목 추가

🤝 기여
기여를 환영합니다! 풀 리퀘스트를 자유롭게 제출해 주세요.

프로젝트 포크

기능 브랜치 생성 (git checkout -b feature/AmazingFeature)

변경 사항 커밋 (git commit -m 'Add some AmazingFeature')

브랜치에 푸시 (git push origin feature/AmazingFeature)

풀 리퀘스트 열기

📝 라이선스
이 프로젝트는 MIT 라이선스 하에 라이선스가 부여됩니다 - 자세한 내용은 LICENSE 파일을 참조하세요.

👤 저자
zayoka

GitHub: @zayoka

🙏 감사의 말
현대 웹 디자인 트렌드에서 영감

아이콘은 Google Material Design에서

파비콘 서비스는 DuckDuckGo (주) 및 Google s2 (대체)

일일 배경화면은 Bing에서 제공

Español
✨ Características
🎨 Tema Oscuro Moderno: Hermoso diseño de glassmorphism con animaciones suaves

🔍 Búsqueda Multi-Motor: Soporte incorporado para Google, Bing y DuckDuckGo

⚙️ Motores de Búsqueda Personalizados: Agrega tus propios motores de búsqueda con URLs personalizadas

🔖 Accesos Directos Rápidos: Crea accesos directos a tus sitios web favoritos con favicons obtenidos automáticamente

🖼️ Fondos de Pantalla Personalizados: Sube tus propias imágenes de fondo (hasta 50MB, 50MP) con soporte de arrastrar y soltar

🌅 Fondo de Pantalla Diario de Bing: Hermosos fondos de pantalla diarios de Bing con caché inteligente de 24 horas y precarga

⚡ Procesamiento de Imágenes de Alto Rendimiento: Soporte para Web Worker, vista previa progresiva y compresión inteligente

🌍 Multi-idioma: Inglés, Chino Simplificado, Chino Tradicional, Japonés, Español, Francés, Coreano

♿ Accesibilidad: Temas de alto contraste, controles de fuente, configuraciones de animación, atajos de teclado

⌨️ Atajos de Teclado: Cambio rápido de motor (Alt+↑↓), enfoque en búsqueda (/), abrir configuración (Alt+,)

💾 Caché Inteligente: Caché de iconos, caché de fondos de pantalla y caché de resultados de procesamiento para carga más rápida

🎯 Limpio y Mínimo: Interfaz sin distracciones centrada en lo importante

🌐 Cambio de Idioma: Cambio fácil de idioma a través de configuración con detección automática

🚀 Instalación
Desde el Código Fuente
Clona este repositorio:

bash
git clone https://github.com/zayokami/GenresFox.git
Abre Chrome/Edge y navega a chrome://extensions/

Habilita el "Modo desarrollador" en la esquina superior derecha

Haz clic en "Cargar extensión descomprimida" y selecciona la carpeta src

¡Disfruta de tu nueva página de pestaña!

Desde Chrome Web Store
Próximamente...

🛠️ Uso
Búsqueda
Simplemente escribe en el cuadro de búsqueda y presiona Enter

Haz clic en el icono del motor de búsqueda para cambiar entre diferentes motores

Las URLs se detectan automáticamente y se abren directamente

Motores de Búsqueda Personalizados
Haz clic en el icono de configuración (⚙️) en la esquina inferior derecha

Ve a la pestaña "Búsqueda y Accesos Directos"

Ingresa el nombre del motor y la URL (usa %s como marcador de posición de consulta de búsqueda)

Ejemplo: https://kagi.com/search?q=%s

Haz clic en "Agregar"

Accesos Directos
Abre configuración y ve a la pestaña "Búsqueda y Accesos Directos"

Desplázate a la sección "Accesos Directos"

Ingresa el nombre y la URL de tu sitio web favorito

El favicon se obtendrá automáticamente

Fondo de Pantalla Personalizado
Abre configuración y ve a la pestaña "Fondo de Pantalla"

Arrastra y suelta una imagen o haz clic para subir

Tamaño máximo de archivo: 50MB, resolución máxima: 50 megapíxeles

Las imágenes se optimizan y comprimen automáticamente para mayor eficiencia de almacenamiento

Haz clic en "Restablecer a Predeterminado" para restaurar el fondo original

Cambio de Idioma
Haz clic en el icono de configuración (⚙️) en la esquina inferior derecha

Ve a la pestaña "Apariencia"

Selecciona tu idioma preferido del menú desplegable

La interfaz se actualizará inmediatamente sin necesidad de actualizar

🔧 Desarrollo
Estructura del Proyecto
text
GenresFox/
├── src/
│   ├── _locales/           # Archivos de internacionalización
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # Icono de extensión
│   ├── manifest.json       # Manifiesto de extensión
│   ├── newtab.html         # Archivo HTML principal
│   ├── script.js           # Lógica principal de JavaScript
│   ├── search.js           # Lógica de barra de búsqueda y botones
│   ├── i18n.js             # Módulo de internacionalización
│   ├── wallpaper.js        # Módulo de gestión de fondos de pantalla
│   ├── accessibility.js    # Módulo de funciones de accesibilidad
│   ├── image-processor.js  # Módulo de procesamiento de imágenes de alto rendimiento
│   ├── image-worker.js     # Web Worker para procesamiento de imágenes en segundo plano
│   ├── styles.css          # Estilos principales
│   ├── search.css          # Estilos de barra de búsqueda
│   └── accessibility.css   # Estilos de accesibilidad
├── CHANGELOG.md
└── README.md
Tecnologías Utilizadas
Manifest V3: Estándar más reciente de extensiones de Chrome

Vanilla JavaScript: Sin frameworks, rendimiento puro

CSS3: Estilizado moderno con efectos de glassmorphism

Web Workers: Procesamiento de imágenes en segundo plano sin bloquear la UI

IndexedDB: Para almacenar archivos grandes de fondos de pantalla y caché

LocalStorage: Para configuraciones persistentes y caché de metadatos

Chrome Extension APIs: Para internacionalización e integración del navegador

Agregar Nuevos Idiomas
Crea una nueva carpeta en src/_locales/ con el código de idioma (ej., fr para francés)

Copia messages.json de la carpeta en

Traduce todos los valores de mensaje

Agrega el idioma a _fallbackMessages en src/i18n.js

Actualiza el arreglo _supportedLanguages y la función _detectLanguage()

Agrega una entrada de cambio de idioma en la UI de configuración

🤝 Contribuciones
¡Las contribuciones son bienvenidas! No dudes en enviar un Pull Request.

Haz un fork del proyecto

Crea tu rama de funcionalidad (git checkout -b feature/AmazingFeature)

Confirma tus cambios (git commit -m 'Add some AmazingFeature')

Sube a la rama (git push origin feature/AmazingFeature)

Abre un Pull Request

📝 Licencia
Este proyecto está bajo la Licencia MIT - consulta el archivo LICENSE para más detalles.

👤 Autor
zayoka

GitHub: @zayoka

🙏 Agradecimientos
Inspirado por tendencias modernas de diseño web

Iconos de Google Material Design

Servicio de favicon por DuckDuckGo (principal) y Google s2 (alternativa)

Fondos de pantalla diarios por Bing

Français
✨ Fonctionnalités
🎨 Thème Sombre Moderne: Beau design glassmorphism avec des animations fluides

🔍 Recherche Multi-Moteurs: Prise en charge intégrée de Google, Bing et DuckDuckGo

⚙️ Moteurs de Recherche Personnalisés: Ajoutez vos propres moteurs de recherche avec des URLs personnalisées

🔖 Raccourcis Rapides: Créez des raccourcis vers vos sites web préférés avec favicons récupérés automatiquement

🖼️ Fond d'Écran Personnalisé: Téléchargez vos propres images de fond (jusqu'à 50MB, 50MP) avec prise en charge du glisser-déposer

🌅 Fond d'Écran Quotidien Bing: De beaux fonds d'écran quotidiens de Bing avec mise en cache intelligente de 24 heures et préchargement

⚡ Traitement d'Image Haute Performance: Prise en charge des Web Workers, prévisualisation progressive et compression intelligente

🌍 Multi-langue: Anglais, Chinois Simplifié, Chinois Traditionnel, Japonais, Espagnol, Français, Coréen

♿ Accessibilité: Thèmes à haut contraste, contrôles de police, paramètres d'animation, raccourcis clavier

⌨️ Raccourcis Clavier: Changement rapide de moteur (Alt+↑↓), focus sur la recherche (/), ouvrir les paramètres (Alt+,)

💾 Mise en Cache Intelligente: Mise en cache d'icônes, de fonds d'écran et de résultats de traitement pour un chargement plus rapide

🎯 Propre et Minimal: Interface sans distraction axée sur l'essentiel

🌐 Changement de Langue: Changement facile de langue via les paramètres avec détection automatique

🚀 Installation
À partir du Code Source
Clonez ce dépôt :

bash
git clone https://github.com/zayokami/GenresFox.git
Ouvrez Chrome/Edge et naviguez vers chrome://extensions/

Activez le "Mode développeur" dans le coin supérieur droit

Cliquez sur "Charger l'extension non empaquetée" et sélectionnez le dossier src

Profitez de votre nouvelle page d'onglet !

Depuis le Chrome Web Store
Bientôt disponible...

🛠️ Utilisation
Recherche
Tapez simplement dans la zone de recherche et appuyez sur Entrée

Cliquez sur l'icône du moteur de recherche pour basculer entre différents moteurs

Les URLs sont automatiquement détectées et ouvertes directement

Moteurs de Recherche Personnalisés
Cliquez sur l'icône des paramètres (⚙️) en bas à droite

Allez dans l'onglet "Recherche et Raccourcis"

Entrez le nom du moteur et l'URL (utilisez %s comme espace réservé pour la requête de recherche)

Exemple : https://kagi.com/search?q=%s

Cliquez sur "Ajouter"

Raccourcis
Ouvrez les paramètres et allez dans l'onglet "Recherche et Raccourcis"

Faites défiler jusqu'à la section "Raccourcis"

Entrez le nom et l'URL de votre site web préféré

Le favicon sera récupéré automatiquement

Fond d'Écran Personnalisé
Ouvrez les paramètres et allez dans l'onglet "Fond d'écran"

Glissez-déposez une image ou cliquez pour télécharger

Taille maximale du fichier : 50MB, résolution maximale : 50 mégapixels

Les images sont automatiquement optimisées et compressées pour une efficacité de stockage

Cliquez sur "Rétablir la valeur par défaut" pour restaurer l'arrière-plan d'origine

Changement de Langue
Cliquez sur l'icône des paramètres (⚙️) en bas à droite

Allez dans l'onglet "Apparence"

Sélectionnez votre langue préférée dans le menu déroulant

L'interface sera mise à jour immédiatement sans actualisation

🔧 Développement
Structure du Projet
text
GenresFox/
├── src/
│   ├── _locales/           # Fichiers d'internationalisation
│   │   ├── en/
│   │   ├── es/
│   │   ├── fr/
│   │   ├── ja/
│   │   ├── ko/
│   │   ├── zh_CN/
│   │   └── zh_TW/
│   ├── icon.png            # Icône de l'extension
│   ├── manifest.json       # Manifeste de l'extension
│   ├── newtab.html         # Fichier HTML principal
│   ├── script.js           # Logique JavaScript principale
│   ├── search.js           # Logique de la barre de recherche et des boutons
│   ├── i18n.js             # Module d'internationalisation
│   ├── wallpaper.js        # Module de gestion des fonds d'écran
│   ├── accessibility.js    # Module de fonctionnalités d'accessibilité
│   ├── image-processor.js  # Module de traitement d'image haute performance
│   ├── image-worker.js     # Web Worker pour le traitement d'image en arrière-plan
│   ├── styles.css          # Styles principaux
│   ├── search.css          # Styles de la barre de recherche
│   └── accessibility.css   # Styles d'accessibilité
├── CHANGELOG.md
└── README.md
Technologies Utilisées
Manifest V3: Dernière norme d'extension Chrome

Vanilla JavaScript: Sans frameworks, performances pures

CSS3: Style moderne avec effets glassmorphism

Web Workers: Traitement d'image en arrière-plan sans bloquer l'interface utilisateur

IndexedDB: Pour stocker les fichiers de fond d'écran volumineux et le cache

LocalStorage: Pour les paramètres persistants et la mise en cache des métadonnées

Chrome Extension APIs: Pour l'internationalisation et l'intégration du navigateur

Ajouter de Nouvelles Langues
Créez un nouveau dossier dans src/_locales/ avec le code de langue (ex. fr pour le français)

Copiez messages.json depuis le dossier en

Traduisez toutes les valeurs de messages

Ajoutez la langue à _fallbackMessages dans src/i18n.js

Mettez à jour le tableau _supportedLanguages et la fonction _detectLanguage()

Ajoutez une entrée de changement de langue dans l'interface utilisateur des paramètres

🤝 Contributions
Les contributions sont les bienvenues ! N'hésitez pas à soumettre une Pull Request.

Forkez le projet

Créez votre branche de fonctionnalité (git checkout -b feature/AmazingFeature)

Committez vos modifications (git commit -m 'Add some AmazingFeature')

Poussez vers la branche (git push origin feature/AmazingFeature)

Ouvrez une Pull Request

📝 Licence
Ce projet est sous licence MIT - voir le fichier LICENSE pour plus de détails.

👤 Auteur
zayoka

GitHub : @zayoka

🙏 Remerciements
Inspiré par les tendances modernes de conception web

Icônes de Google Material Design

Service de favicon par DuckDuckGo (principal) et Google s2 (alternative)

Fonds d'écran quotidiens par Bing


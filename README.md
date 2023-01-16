# 環境の構築手順

### 仮想環境構築
1. % python3 -m venv 仮想環境名
2. % source 仮想環境名/bin/activate
3. % python -m pip install Django *仮想環境上にDjangoインストール
4. % deactivate で仮想環境から抜ける

### projectの作成
1. % mkdir test
2. % cd test
3. % django-admin startproject todoproject .
4. % python manage.py startapp todo

### 初期設定
1. todoproject/settings.pyで、TEMPLATES[]内の、'DIRS': [BASE_DIR / 'templates']と記述場所を指定
2. アプリを作成したため、todoproject/settings.pyで、INSTALLED_APPS[]内に、'todo.apps.TodoConfig'を記載

### サーバーの起動
1. % python manage.py runserver
2. urlを貼り付ける

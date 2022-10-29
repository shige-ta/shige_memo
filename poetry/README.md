powershell でインストール

pyenv インストール

```bash
Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"
```

```bash
pyenv --version
pyenv install -l
pyenv install <version>
pyenv global <version>
```

poetry インストール

```bash
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -
```

新規作成のプロジェクト

```bash
poetry new <project-name>
```

既存プロジェクト

```bash
poetry init
```

パッケージインストール

```bash
poetry add <パッケージ名>
```

仮想環境で python のプログラムを実行

```bash
poetry run python <****.py>
```

pytest 実行

```bash
poetry run pytest
```

↓ 参考サイト
Poetry documentation (ver. 1.1.6 日本語訳)
https://cocoatomo.github.io/poetry-ja/

Poetry をサクッと使い始めてみる - Qiita
https://qiita.com/ksato9700/items/b893cf1db83605898d8a

Introduction | Documentation | Poetry - Python dependency management and packaging made easy
https://python-poetry.org/docs/#installing-with-the-official-installer

pyenv-win/pyenv-win: pyenv for Windows. pyenv is a simple python version management tool. It lets you easily switch between multiple versions of Python. It's simple, unobtrusive, and follows the UNIX tradition of single-purpose tools that do one thing well.
https://github.com/pyenv-win/pyenv-win

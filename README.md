*This project has been created as part of the 42 curriculum by hwakatsu.*

# Data Archivist

## Description / 説明

### English
Data Archivist is a Python project about file operations, stream handling, context managers, and error handling. Its goal is to practice the core techniques needed to safely read files, create files, communicate through standard streams, protect resources with `with`, and respond gracefully to archive-access failures.

This repository contains five exercises:

- `ex0/ft_ancient_text.py`: reads an archive file and reports recovery status
- `ex1/ft_archive_creation.py`: creates a new archive file and writes preservation entries
- `ex2/ft_stream_management.py`: demonstrates `stdin`, `stdout`, and `stderr`
- `ex3/ft_vault_security.py`: uses `with` statements for secure file operations
- `ex4/ft_crisis_response.py`: handles normal and failing file-access scenarios with exceptions

From the code in this repository, the project demonstrates:

- manual file opening, reading, writing, and closing
- safe resource management with context managers
- standard output and error-channel separation
- exception handling for missing files, permission issues, and unexpected failures

### 日本語
Data Archivist は、ファイル操作、標準ストリーム管理、context manager、例外処理を学ぶ Python プロジェクトです。目的は、ファイルの安全な読み込み、ファイル作成、標準入出力の使い分け、`with` によるリソース保護、そしてアーカイブアクセス失敗時の適切な対応を実践することです。

このリポジトリには 5 つの exercise があります。

- `ex0/ft_ancient_text.py`: アーカイブファイルを読み込み、復旧状況を表示する
- `ex1/ft_archive_creation.py`: 新しいアーカイブファイルを作成し、保存データを書き込む
- `ex2/ft_stream_management.py`: `stdin`、`stdout`、`stderr` を実演する
- `ex3/ft_vault_security.py`: `with` 文を使って安全なファイル操作を行う
- `ex4/ft_crisis_response.py`: 通常ケースと失敗ケースのファイルアクセスを例外処理で扱う

このリポジトリの実装では、次の内容が確認できます。

- 手動でのファイル open、read、write、close
- context manager を使った安全なリソース管理
- 標準出力とエラーチャンネルの分離
- ファイル未発見、権限エラー、予期しない失敗への例外処理

## Instructions / 実行方法

### English

Requirements:

- Python 3.10 or later
- No external dependencies

Run each exercise from the repository root:

```bash
python3 ex0/ft_ancient_text.py
python3 ex1/ft_archive_creation.py
python3 ex2/ft_stream_management.py
python3 ex3/ft_vault_security.py
python3 ex4/ft_crisis_response.py
```

Optional lint check:

```bash
flake8 ex0 ex1 ex2 ex3 ex4
```

Some exercises expect local test files to exist:

- `ex0` reads `ancient_fragment.txt`
- `ex3` reads `classified_data.txt` and writes `preserving_new_information.txt`
- `ex4` attempts access to `lost_archive.txt`, `classified_vault.txt`, and `standard_archive.txt`

There is no compilation or installation step. The project uses only the Python standard library.

### 日本語

必要環境:

- Python 3.10 以上
- 外部依存関係なし

リポジトリのルートで、各 exercise は次のように実行できます。

```bash
python3 ex0/ft_ancient_text.py
python3 ex1/ft_archive_creation.py
python3 ex2/ft_stream_management.py
python3 ex3/ft_vault_security.py
python3 ex4/ft_crisis_response.py
```

任意の lint チェック:

```bash
flake8 ex0 ex1 ex2 ex3 ex4
```

一部の exercise はローカルファイルの存在を前提としています。

- `ex0` は `ancient_fragment.txt` を読み込みます
- `ex3` は `classified_data.txt` を読み込み、`preserving_new_information.txt` を書き込みます
- `ex4` は `lost_archive.txt`、`classified_vault.txt`、`standard_archive.txt` へのアクセスを試みます

コンパイルやインストールは不要です。このプロジェクトは Python 標準ライブラリのみを使用します。

## Features / 主な内容

### English

- File reading with explicit `open()` / `close()`
- File writing with archive-style status output
- Interactive input handling with `sys.stdout` and `sys.stderr`
- Context-manager based secure vault access
- Crisis-response style exception handling for file operations

### 日本語

- `open()` / `close()` を明示したファイル読み込み
- アーカイブ風の状態表示を伴うファイル書き込み
- `sys.stdout` と `sys.stderr` を使った対話入力処理
- context manager を使った安全な vault アクセス
- ファイル操作に対する crisis-response 形式の例外処理

## Usage Overview / 使い方の概要

### English

- `ex0` focuses on reading and graceful failure when a file is missing.
- `ex1` focuses on creating a file and writing fixed archive entries.
- `ex2` focuses on stream separation and interactive messaging.
- `ex3` focuses on automatic resource cleanup with `with`.
- `ex4` focuses on crisis handling for successful and failed archive access.

### 日本語

- `ex0` はファイル読み込みと、ファイル欠如時の適切な失敗処理に焦点があります。
- `ex1` はファイル作成と固定エントリの書き込みに焦点があります。
- `ex2` はストリーム分離と対話メッセージ処理に焦点があります。
- `ex3` は `with` による自動リソース解放に焦点があります。
- `ex4` は成功ケースと失敗ケースを含むアーカイブアクセスの危機対応に焦点があります。

## Resources / 参考資料

### English

Classic references related to the topic:

- [Python Documentation: open()](https://docs.python.org/3/library/functions.html#open)
- [Python Documentation: Input and Output](https://docs.python.org/3/tutorial/inputoutput.html)
- [Python Documentation: with Statement](https://docs.python.org/3/reference/compound_stmts.html#the-with-statement)
- [Python Documentation: Exceptions](https://docs.python.org/3/tutorial/errors.html)
- [Python Documentation: sys](https://docs.python.org/3/library/sys.html)
- [Real Python: Working With Files in Python](https://realpython.com/working-with-files-in-python/)
- [flake8 Documentation](https://flake8.pycqa.org/)

AI usage in this project:

- AI was used for documentation support and README drafting.
- It was used to inspect the repository structure, summarize the behavior of the five exercises, and provide bilingual English/Japanese wording.
- The README was aligned with the code in `ex0` through `ex4`, but the implementation and required local test files should still be checked manually before submission and peer review.

### 日本語

この課題に関連する代表的な参考資料:

- [Python Documentation: open()](https://docs.python.org/3/library/functions.html#open)
- [Python Documentation: Input and Output](https://docs.python.org/3/tutorial/inputoutput.html)
- [Python Documentation: with Statement](https://docs.python.org/3/reference/compound_stmts.html#the-with-statement)
- [Python Documentation: Exceptions](https://docs.python.org/3/tutorial/errors.html)
- [Python Documentation: sys](https://docs.python.org/3/library/sys.html)
- [Real Python: Working With Files in Python](https://realpython.com/working-with-files-in-python/)
- [flake8 Documentation](https://flake8.pycqa.org/)

このプロジェクトにおける AI の利用:

- AI はドキュメント補助と README 作成支援に使用しました。
- リポジトリ構造の確認、5 つの exercise の挙動要約、英語と日本語の文章作成に利用しました。

## Notes / 補足

### English
This project emphasizes reliable fundamentals rather than complex business logic. The main point is to show safe file handling and stable behavior when operations succeed or fail.

### 日本語
このプロジェクトは複雑な業務ロジックよりも、信頼できる基礎操作を重視しています。主眼は、ファイル操作が成功する場合も失敗する場合も、安全に扱えることを示す点にあります。

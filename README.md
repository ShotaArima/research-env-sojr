# research-env-sojr
## `uv`の環境構築方法
1. ローカルに`uv`をinstallする

```powershell
# Windows
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

2. `uv`で仮想環境を作成する
```
uv create (my_env)

# activateする
uv activate my_env
```

3. `uv`でpythonをinstallする
```
uv python install (バージョン)
```

4. スクリプトの実行
```
uv run main.py
```

5. 必要なライブラリのinstall
```
uv add (ライブラリ名==バージョン)
```
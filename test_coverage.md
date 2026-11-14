# 測試覆蓋度：LoadDensity

測量日期：2026-10-28。數字來自這台 Windows 機器上的一次實測，不是估計，也不是只數檔案。

| 項目 | 內容 |
|---|---|
| 直譯器 | 3.11.9 |
| 直譯器說明 | 專案 .venv |
| 工具 | coverage 7.15.0，`coverage run --branch` |
| 測量範圍 | `je_load_density` |
| 測試路徑 | `test` |
| 命令 | `python -m coverage run --branch --source=je_load_density -m pytest test` |
| 敘述覆蓋 | 85.48%（10500 / 12283） |
| 分支覆蓋 | 76.53%（2544 / 3324） |
| 測試結果 | 1628 passed, 14 skipped, 4 warnings in 130.39s (0:02:10) |
| 耗時 | 134.0 秒 |

敘述覆蓋是執行到的敘述數除以全部敘述數。分支覆蓋是執行到的分支數除以全部分支數。兩者分開算，沒有把分支混進敘述百分比。

## 覆蓋較低的檔案

只列這次測量裡敘述覆蓋最低的檔案，最多 12 個。

| 檔案 | 敘述覆蓋 | 已覆蓋 / 敘述 |
|---|---:|---:|
| `je_load_density/utils/metrics/opentelemetry_tracing_exporter.py` | 0.0% | 0 / 66 |
| `je_load_density/utils/recording/cdp_capture.py` | 0.0% | 0 / 66 |
| `je_load_density/utils/metrics/datadog_apm_exporter.py` | 0.0% | 0 / 60 |
| `je_load_density/utils/recording/mitmproxy_addon.py` | 0.0% | 0 / 42 |
| `je_load_density/engine/bench_cli.py` | 0.0% | 0 / 30 |
| `je_load_density/gui/main_window.py` | 0.0% | 0 / 27 |
| `je_load_density/utils/json/json_format/json_process.py` | 0.0% | 0 / 23 |
| `je_load_density/utils/file_process/create_project_structure.py` | 0.0% | 0 / 13 |
| `je_load_density/utils/get_data_structure/get_api_data.py` | 0.0% | 0 / 12 |
| `je_load_density/action_lsp/__main__.py` | 0.0% | 0 / 5 |
| `je_load_density/mcp_server/__main__.py` | 0.0% | 0 / 5 |
| `je_load_density/utils/metrics/opentelemetry_exporter.py` | 15.15% | 10 / 66 |

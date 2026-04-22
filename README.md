# 使用说明书

## 项目结构

``` bash
py_dashboard/
├── venv/                            ← 一个虚拟环境，共享
├── shared/                          ← 公共代码（可选）
├── streamlit/                       ← 样式配置
│   └── config.toml                  ← 配置文件
├── requirements.txt                 ← 包依赖文件配置
├── launcher.py                      ← 一个启动入口
├── shared/                          ← 公共代码（可选）
│   └── db.py
├── sales/                           ← 销售看板
│   ├── machine/                     **洗衣机月度营收**
│       └── data
│       └── app.py
├── ops/                             ← 运营看板
│   ├── clean/                       **保洁照片查询**
│       └── app.py
└── finance/                         ← 财务看板
    ├── app.py
    └── .streamlit/config.toml
``` 

##  Reader完整配置示例

| 配置项 | 值 | 说明 |
|--------|-----|------|
| Root Directory | `sales/machine/` | 指定应用所在目录 |
| Build Command | `pip install -r ../../requirements.txt` | 安装依赖 |
| Start Command | `streamlit run app.py --server.port 10000 --server.address 0.0.0.0` | 启动应用 |





## 访问路径

### 洗衣机看板

``` bash
streamlit run sales/machine/app.py
```
https://machine2025.streamlit.app/

### 保洁照片查询看板

``` bash
streamlit run ops/clean/app.py
```
https://cleancheck.streamlit.app/

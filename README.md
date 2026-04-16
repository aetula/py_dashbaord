my_project/
├── venv/                            ← 一个虚拟环境，共享
├── requirements.txt                 ← 一个依赖文件
├── launcher.py                      ← 一个启动入口
├── shared/                          ← 公共代码（可选）
│   └── db.py
├── sales/                           ← 销售看板
│   ├── app.py
│   └── .streamlit/config.toml
├── ops/                             ← 运营看板
│   ├── app.py
│   └── .streamlit/config.toml
└── finance/                         ← 财务看板
    ├── app.py
    └── .streamlit/config.toml
# 🗄️ SQL Database Management Scripts

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=19,2,27&height=210&section=header&text=SQL%20Database%20Management%20Scripts&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Automate%20Backups%2C%20Migrations%20%26%20Maintenance&descAlignY=56&descSize=18" width="100%"/>

<br/>

[![Version](https://img.shields.io/badge/version-5.2.0-4A4E69?style=for-the-badge&logo=semanticrelease&logoColor=white)](https://github.com)
[![Databases](https://img.shields.io/badge/PostgreSQL%20%7C%20MySQL%20%7C%20SQLite-9A8C98?style=for-the-badge&logo=postgresql&logoColor=white)](https://github.com)
[![License](https://img.shields.io/badge/license-MIT-C9ADA7?style=for-the-badge&logo=opensourceinitiative&logoColor=black)](LICENSE)
[![Scripts](https://img.shields.io/badge/scripts-90%2B-F2E9E4?style=for-the-badge&logo=gnubash&logoColor=black)](https://github.com)

<br/>

### 🛠️ A battle-tested collection of SQL scripts for real-world database operations

*💾 Backups • 🔄 Migrations • 📊 Monitoring • 🧹 Cleanup • 🔐 Security*

<br/>

<a href="https://share.google/uoaHVZqzTmQ2uCAe1">
  <img src="https://img.shields.io/badge/📥_GET_SCRIPTS-4A4E69?style=for-the-badge&logo=github&logoColor=white&labelColor=323549" alt="Get Scripts" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/uoaHVZqzTmQ2uCAe1">
  <img src="https://img.shields.io/badge/🚀_QUICK_START-9A8C98?style=for-the-badge&logo=rocket&logoColor=white&labelColor=6F646E" alt="Quick Start" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/uoaHVZqzTmQ2uCAe1">
  <img src="https://img.shields.io/badge/📚_DOCS-C9ADA7?style=for-the-badge&logo=readthedocs&logoColor=black&labelColor=A08A84" alt="Docs" height="45"/>
</a>

</div>

<img width="1024" height="521" alt="generate-sql-script-1024x521" src="https://github.com/user-attachments/assets/71b29c67-eaae-439c-970d-a6fa6dd9d940" />


<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🌟 About

**SQL Database Management Scripts** is a curated, production-ready toolkit of **90+ SQL and shell scripts** that handle the day-to-day realities of running databases: backups, restores, migrations, index maintenance, monitoring, cleanup, and security audits.

No more reinventing the same `pg_dump` cron job or writing another ad-hoc query for finding slow tables — it's all here, tested and documented.

> 💡 **Perfect for:** DBAs, backend developers, DevOps engineers, and anyone maintaining PostgreSQL, MySQL, MariaDB, or SQLite in production.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎯 What's Included

<div align="center">

| 💾 **Backup & Restore** | 🔄 **Migrations** | 📊 **Monitoring** |
|:---:|:---:|:---:|
| Full, incremental,<br/>and point-in-time | Versioned, idempotent<br/>schema changes | Slow queries, locks,<br/>connections, bloat |

| 🧹 **Cleanup** | 🔐 **Security** | ⚙️ **Maintenance** |
|:---:|:---:|:---:|
| Old data pruning,<br/>vacuum, log rotation | User audits, role<br/>grants, password rules | Reindexing, analyze,<br/>statistics refresh |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🏆 Why This Toolkit

<div align="center">

| 💎 **Advantage** | 📝 **Description** |
|:---|:---|
| ✅ **Production-Ready** | Every script is tested against real workloads and edge cases |
| 🎯 **Multi-Engine** | Unified syntax across PostgreSQL, MySQL, MariaDB & SQLite where possible |
| 📖 **Fully Documented** | Each script has a header explaining purpose, inputs, and safety notes |
| 🛡️ **Safe by Default** | Destructive scripts require explicit `--force` flags and create backups first |
| 🔄 **Idempotent** | Re-running any migration or maintenance script never breaks your DB |
| 🧩 **Composable** | Scripts are modular — chain them in your own automations or cron jobs |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎬 Toolkit Preview

<div align="center">

```ascii
╔══════════════════════════════════════════════════╗
║  🗄️  SQL Database Management Scripts  v5.2.0     ║
╠══════════════════════════════════════════════════╣
║                                                  ║
║  📂 backup/                                      ║
║    ├ pg_full_backup.sh      ✅ tested            ║
║    ├ pg_incremental.sh      ✅ tested            ║
║    └ restore_latest.sh      ⚠️  needs --confirm  ║
║                                                  ║
║  📂 monitoring/                                  ║
║    ├ slow_queries.sql       ✅ tested            ║
║    ├ active_locks.sql       ✅ tested            ║
║    └ connection_pool.sql    ✅ tested            ║
║                                                  ║
║  📂 maintenance/                                 ║
║    ├ vacuum_analyze.sh      ✅ tested            ║
║    └ reindex_bloated.sql    ✅ tested            ║
║                                                  ║
║  ⚡ 90 scripts   🛡️ safe-mode ON   📖 100% doc'd ║
╚══════════════════════════════════════════════════╝
```

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧩 Project Structure

```
🗄️ sql-database-management-scripts/
├── 💾 backup/                 # Backup & restore scripts
│   ├── pg_full_backup.sh
│   ├── pg_incremental.sh
│   └── restore_latest.sh
├── 🔄 migrations/             # Versioned schema changes
│   ├── postgres/
│   ├── mysql/
│   └── sqlite/
├── 📊 monitoring/             # Health & performance checks
│   ├── slow_queries.sql
│   ├── active_locks.sql
│   └── bloat_report.sql
├── 🧹 cleanup/                # Data pruning & rotation
├── 🔐 security/               # User audits & grants
├── ⚙️  maintenance/            # Vacuum, reindex, analyze
├── 🧪 tests/                  # Script validation suite
└── 📖 docs/                   # Usage & safety guide
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🛠️ Tech Stack

<div align="center">

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🤝 Community

Found a bug? Have a script idea? Want to add support for a new engine?

<div align="center">

<a href="https://share.google/uoaHVZqzTmQ2uCAe1">
  <img src="https://img.shields.io/badge/💬_Join_Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="35"/>
</a>
<a href="https://share.google/uoaHVZqzTmQ2uCAe1">
  <img src="https://img.shields.io/badge/🐞_Report_Issue-4A4E69?style=for-the-badge&logo=github&logoColor=white" height="35"/>
</a>
<a href="https://share.google/uoaHVZqzTmQ2uCAe1">
  <img src="https://img.shields.io/badge/⭐_Star_Repo-C9ADA7?style=for-the-badge&logo=github&logoColor=black" height="35"/>
</a>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

> **Safety note:** Always test scripts on a staging database before running them in production. Review the header of each script for `--force` and `--dry-run` options.

<br/>

<div align="center">

### 🗄️ Made with 💾 by the SQL Scripts Team

*If these scripts saved you an afternoon — star the repo!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=19,2,27&height=120&section=footer" width="100%"/>

</div>

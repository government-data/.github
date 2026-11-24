# Government Data

**A platform for an organisation's data, installed on servers the
organisation controls.** Government Data brings together the applications
that measure, process and show that data: one sign-in, one set of
permissions, one audit trail and one data lake.

## Why it exists

Organisations need to trust their data before they decide with it. Government
Data lets the people who know the data write the rules it must meet, measures
it on a schedule, shows where it fails and who must fix it, and keeps every
copy and every result inside the organisation's own installation.

- **Your data stays with you.** One installation serves one organisation, and
  no data leaves it except what the organisation exports.
- **Updates are pulled, never pushed.** Each installation fetches signed
  versions, checks the signature, backs up and applies them. Nothing reaches
  into an installation from outside.
- **Open formats.** Data and results live as open Apache Iceberg tables,
  queried with standard SQL.
- **Modular.** Each application is a module that can be added, and removed
  without losing its data.

## Applications and modules

| | What it is for |
| --- | --- |
| **Quality Data** | Data quality: rules, cuts that measure the data, indicators and remediation queues |
| **Orchestrator** | Schedules and tracks the platform's jobs; its workers run them |
| **Analytics** | Dashboards of the indicators, with Apache Superset |
| **Data lake** | Open tables on RustFS and Apache Iceberg, queried through Trino |
| **User guide** | Served inside every installation and published openly |

## Repositories

| Repository | What it holds |
| --- | --- |
| [core](https://github.com/quality-data/core) | The platform's core and the Quality Data application |
| [quality-sdk](https://github.com/quality-data/quality-sdk) | Installs, configures and updates an installation and its modules from signed versions |
| [lake-rustfs](https://github.com/quality-data/lake-rustfs) | The data lake module on RustFS |
| [query-trino](https://github.com/quality-data/query-trino) | The SQL query module on Trino |
| [docs](https://github.com/quality-data/docs) | The user guide |

## Learn more

The user guide, in English and Spanish: **https://orquestador.app**

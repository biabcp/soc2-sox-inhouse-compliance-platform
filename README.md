# soc2-sox-inhouse-compliance-platform
A reference implementation of an in-house compliance automation platform for SOC 2 and SOX, including infra-as-code, control-as-code, and evidence pipelines. 

soc2-sox-inhouse-compliance-platform/
├── README.md
├── docs/
│   ├── 00-intro.md
│   ├── 01-architecture.md
│   ├── 02-soc2-overview.md
│   ├── 03-sox-overview.md
│   ├── 04-control-mapping.md
│   ├── 05-deployment-guide.md
│   └── 06-auditor-guide.md
├── controls/
│   ├── soc2/
│   │   ├── cc1_1.yml
│   │   ├── cc2_1.yml
│   │   └── ...
│   ├── sox/
│   │   ├── itgc-access.yml
│   │   ├── itgc-change-mgmt.yml
│   │   └── ...
│   └── mappings/
│       └── soc2-sox-mapping.yml
├── evidence/
│   ├── raw/
│   │   ├── github/
│   │   ├── cloud/
│   │   ├── idp/
│   │   └── tickets/
│   └── processed/
│       ├── 2025-01-01/
│       └── 2025-02-01/
├── src/
│   ├── collectors/
│   │   ├── github_collector.py
│   │   ├── cloud_collector.py
│   │   ├── idp_collector.py
│   │   └── tickets_collector.py
│   ├── evaluators/
│   │   ├── control_engine.py
│   │   └── rules/
│   │       ├── soc2_rules.yml
│   │       └── sox_rules.yml
│   ├── reporting/
│   │   ├── generate_dashboard.py
│   │   └── generate_audit_package.py
│   └── utils/
│       └── config.py
├── infra/
│   ├── terraform/
│   │   ├── logging.tf
│   │   ├── security_baseline.tf
│   │   └── iam.tf
│   └── policies/
│       └── example-policies.md
├── .github/
│   └── workflows/
│       ├── nightly-compliance.yml
│       └── pr-gate.yml
├── requirements.txt
└── pyproject.toml (optional if using Poetry)


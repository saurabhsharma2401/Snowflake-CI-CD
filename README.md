
This repository contains the implementation of CI/CD workflow for Snowflake using Azure DevOps and Flyway

The below are included files.
```
├── README.md
├── databases
│   ├── README.md
│   └── flyway_demo
│       ├── V20200120.1__SCHEMA_DEMO_Create.sql
│       ├── V20200120.2__TABLE_DEMO.DEMOTABLE_Create.sql
│       ├── V20200123.1__TABLE_DEMO.DEMOTABLE_Alter.sql
│       └── view
│           └── R__VIEW_DEMO.V_DEMOVIEW.sql
└── templates
    ├── README.md
    ├── TaskGroups
    ├── VariableGroups
    │   ├── Classic
    │   │   └── Snowflake.Database.env      <- Variable group for Classic pipeline
    │   └── YAML
    │       └── Snowflake.Database.env      <- Variable group for YAML pipeline
    └── YAMLpipelines
        ├── azure-pipelines.yml             <- YAML pipeline script
        └── templates
            ├── snowflakeFlywayBuild.yml    <- YAML pipeline template for snowflake build using flyway
            └── snowflakeFlywayDeploy.yml   <- YAML pipeline template for snowflake deploy using flyway
```

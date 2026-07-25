---
api_specs:
- filename: amazon-glue-databrew-datasets-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew Datasets API
  slug: amazon-glue-databrew-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-datasets-api-openapi.yml
- filename: amazon-glue-databrew-jobs-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew Jobs API
  slug: amazon-glue-databrew-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-jobs-api-openapi.yml
- filename: amazon-glue-databrew-profilejobs-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew ProfileJobs API
  slug: amazon-glue-databrew-profilejobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-profilejobs-api-openapi.yml
- filename: amazon-glue-databrew-projects-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew Projects API
  slug: amazon-glue-databrew-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-projects-api-openapi.yml
- filename: amazon-glue-databrew-recipejobs-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew RecipeJobs API
  slug: amazon-glue-databrew-recipejobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-recipejobs-api-openapi.yml
- filename: amazon-glue-databrew-recipes-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew Recipes API
  slug: amazon-glue-databrew-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-recipes-api-openapi.yml
- filename: amazon-glue-databrew-recipeversions-name-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew RecipeVersions#name API
  slug: amazon-glue-databrew-recipeversions-name-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-recipeversions-name-api-openapi.yml
- filename: amazon-glue-databrew-rulesets-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew Rulesets API
  slug: amazon-glue-databrew-rulesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-rulesets-api-openapi.yml
- filename: amazon-glue-databrew-schedules-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew Schedules API
  slug: amazon-glue-databrew-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-schedules-api-openapi.yml
- filename: amazon-glue-databrew-tags-api-openapi.yml
  format: yaml
  label: Amazon Glue DataBrew Tags API
  slug: amazon-glue-databrew-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/openapi/amazon-glue-databrew-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: databrew.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Glue Databrew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Glue DataBrew, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
slug: amazon-glue-databrew-domain-security
source_filename: amazon-glue-databrew-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: databrew.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/security/amazon-glue-databrew-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
---

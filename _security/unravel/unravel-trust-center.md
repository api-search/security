---
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Unravel Trust Center
name_suffix: Trust Center
overview: Unravel maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Unravel
provider_slug: unravel
slug: unravel-trust-center
source_filename: unravel-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nsource: https://trust.unraveldata.com/\nurl: https://trust.unraveldata.com/\nplatform: Conveyor\ncertifications:\n- SOC 2 Type II\nevidence:\n- source: https://trust.unraveldata.com/\n  kind: trust-center\n  detail: Conveyor-powered trust center; Unravel's own company record in the page\n    payload lists certifications [\"soc2-type-2\"] and page copy states \"Unravel is\n    SOC 2 Type II compliant\". Keyword probes also matched hipaa/fedramp/gdpr/iso-27017/\n    iso-27018 on this page, but those certifications belong to subprocessor entries\n    (e.g. Snowflake) rendered in the same payload, so they are not attributed to\n    Unravel here.\n- source: https://www.unraveldata.com/\n  kind: website-footer\n  detail: Homepage links to https://trust.unraveldata.com/ and to a SOC 2 docs page.\nnotes: Trust center exposes an NDA-gated dataroom for the SOC 2 Type II report. The\n  trust-center metadata had empty reportVulnerabilityUrl,\
  \ securityContact,\n  privacyPolicyUrl, and termsConditionsUrl fields at probe time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unravel/refs/heads/main/security/unravel-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Data Observability
- FinOps
- DataOps
- Cost Optimization
- Databricks
- Snowflake
- BigQuery
- Monitoring
- Company
trust_url: https://trust.unraveldata.com/
---

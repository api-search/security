---
description: ''
domains:
- caa:
  - 0 issuewild "intermediatecertificate.digitalcertvalidation.com"
  - 0 issuewild "letsencrypt.org;validationmethods=dns-01"
  - 0 issuewild "pki.goog"
  - 0 issuewild "rapidssl.com"
  - 0 issuewild "stratossl.digitalcertvalidation.com"
  - 0 issuewild "thawte.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: databricks.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: docs.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <workspace-instance>.cloud.databricks.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Databricks Asset Bundles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databricks Asset Bundles, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Databricks Asset Bundles
provider_slug: databricks-asset-bundles
slug: databricks-asset-bundles-domain-security
source_filename: databricks-asset-bundles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <workspace-instance>.cloud.databricks.com\n  https: false\ndomains:\n- domain: databricks.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"intermediatecertificate.digitalcertvalidation.com\"\n  - 0 issuewild \"letsencrypt.org;validationmethods=dns-01\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"rapidssl.com\"\n  - 0 issuewild \"stratossl.digitalcertvalidation.com\"\n  - 0 issuewild \"thawte.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databricks-asset-bundles/refs/heads/main/security/databricks-asset-bundles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CI/CD
- Data Engineering
- Databricks
- Deployment
- Infrastructure as Code
- Job
- Machine-Learning
- MLOps
- Pipelines
- Workflows
---

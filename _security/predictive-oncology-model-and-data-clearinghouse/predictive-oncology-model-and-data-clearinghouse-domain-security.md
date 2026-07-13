---
api_specs:
- filename: predictive-oncology-model-and-data-clearinghouse-openapi.json
  format: json
  label: MoDaC REST API
  slug: modac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predictive-oncology-model-and-data-clearinghouse/refs/heads/main/openapi/predictive-oncology-model-and-data-clearinghouse-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "identrust.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: true
  domain: cancer.gov
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: modac.cancer.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Predictive Oncology Model And Data Clearinghouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Predictive Oncology Model and Data Clearinghouse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Predictive Oncology Model and Data Clearinghouse
provider_slug: predictive-oncology-model-and-data-clearinghouse
slug: predictive-oncology-model-and-data-clearinghouse-domain-security
source_filename: predictive-oncology-model-and-data-clearinghouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modac.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cancer.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predictive-oncology-model-and-data-clearinghouse/refs/heads/main/security/predictive-oncology-model-and-data-clearinghouse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Cancer Research
- Clinical Data
- Datasets
- Machine Learning
- Oncology
---

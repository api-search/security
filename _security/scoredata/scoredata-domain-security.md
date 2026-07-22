---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scoredata.com
  spf: false
hosts:
- cert_expires: Oct 15 18:02:38 2026 GMT
  host: scoredata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scoredata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScoreData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ScoreData
provider_slug: scoredata
slug: scoredata-domain-security
source_filename: scoredata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scoredata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:02:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scoredata.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scoredata/refs/heads/main/security/scoredata-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Predictive Analytics
- Data Science
- MLOps
- Financial Services
- Insurance
- Healthcare
---

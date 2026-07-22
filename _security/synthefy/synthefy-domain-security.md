---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: synthefy.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.synthefy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 21:48:00 2026 GMT
  host: docs.synthefy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: forecast.synthefy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synthefy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthefy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synthefy
provider_slug: synthefy
slug: synthefy-domain-security
source_filename: synthefy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synthefy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n- host: docs.synthefy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: forecast.synthefy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: synthefy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthefy/refs/heads/main/security/synthefy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Foundation Models
- Machine Learning
- Forecasting
- Time Series
- Tabular Data
- Synthetic Data
- Artificial Intelligence
- Predictive Analytics
---

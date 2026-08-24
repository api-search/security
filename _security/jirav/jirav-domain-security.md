---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jirav.com
  spf: true
hosts:
- cert_expires: Oct 29 05:29:58 2026 GMT
  host: www.jirav.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jirav Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jirav, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jirav
provider_slug: jirav
slug: jirav-domain-security
source_filename: jirav-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jirav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 05:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: jirav.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jirav/refs/heads/main/security/jirav-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Planning
- FP&A
- Budgeting
- Forecasting
- Accounting
- Reporting
- Dashboards
- Business Intelligence
- SaaS
---

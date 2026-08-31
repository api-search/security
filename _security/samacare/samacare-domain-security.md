---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: samacare.com
  spf: true
hosts:
- cert_expires: Oct 15 05:59:35 2026 GMT
  host: www.samacare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 07:43:19 2026 GMT
  host: samacare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: api.samacare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Samacare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SamaCare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SamaCare
provider_slug: samacare
slug: samacare-domain-security
source_filename: samacare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.samacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 05:59:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: samacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:43:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.samacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: samacare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samacare/refs/heads/main/security/samacare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Prior Authorization
- Patient Access
- Specialty Pharmacy
- Life Sciences
- Electronic Health Records
- Revenue Cycle Management
- Market Access
- Artificial Intelligence
---

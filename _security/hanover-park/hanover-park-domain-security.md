---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hanoverpark.com
  spf: true
hosts:
- cert_expires: Oct 14 02:02:20 2026 GMT
  host: www.hanoverpark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hanover Park Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hanover Park, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hanover Park
provider_slug: hanover-park
slug: hanover-park-domain-security
source_filename: hanover-park-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hanoverpark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 02:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hanoverpark.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanover-park/refs/heads/main/security/hanover-park-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Software
- Fund Administration
- Private Equity
- Venture Capital
- Fintech
- Financial Operations
- AI
- ERP
- Back Office
---

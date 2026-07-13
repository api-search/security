---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issuewild ";"
  - 0 issue "amazontrust.com"
  - 0 issue "quovadisglobal.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: abnamro.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.abnamro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: developer.abnamro.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abn Amro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABN AMRO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ABN AMRO
provider_slug: abn-amro
slug: abn-amro-domain-security
source_filename: abn-amro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abnamro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.abnamro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: abnamro.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"quovadisglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abn-amro/refs/heads/main/security/abn-amro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- European Banking
- Open Banking
- PSD2
- Payments
---

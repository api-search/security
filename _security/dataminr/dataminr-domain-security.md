---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dataminr.com
  spf: true
hosts:
- cert_expires: Jan 16 13:02:38 2027 GMT
  host: www.dataminr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 20:29:12 2026 GMT
  host: developer.dataminr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: gateway.dataminr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dataminr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dataminr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dataminr
provider_slug: dataminr
slug: dataminr-domain-security
source_filename: dataminr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dataminr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 13:02:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.dataminr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 20:29:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gateway.dataminr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dataminr.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataminr/refs/heads/main/security/dataminr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Threat Intelligence
- Risk Management
- Real-Time
- Security
- Artificial Intelligence
- Alerting
---

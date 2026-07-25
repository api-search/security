---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onetick.com
  spf: true
hosts:
- cert_expires: Sep  4 20:15:34 2026 GMT
  host: www.onetick.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: authdash.cloud.onetick.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: rest.cloud.onetick.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onetick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneTick (OneMarketData), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OneTick (OneMarketData)
provider_slug: onetick
slug: onetick-domain-security
source_filename: onetick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onetick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:15:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: authdash.cloud.onetick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.cloud.onetick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onetick.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onetick/refs/heads/main/security/onetick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Market Data
- Tick Data
- Historical Data
- Trading
- Analytics
- Surveillance
- Time Series
- Equities
- Options
---

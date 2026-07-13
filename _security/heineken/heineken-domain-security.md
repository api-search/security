---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: theheinekencompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: heineken.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.theheinekencompany.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 04:03:43 2026 GMT
  host: developer.heineken.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heineken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heineken, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Heineken
provider_slug: heineken
slug: heineken-domain-security
source_filename: heineken-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theheinekencompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.heineken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:03:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theheinekencompany.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: heineken.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heineken/refs/heads/main/security/heineken-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Beverages
- Consumer Goods
- Manufacturing
- B2B Integration
---

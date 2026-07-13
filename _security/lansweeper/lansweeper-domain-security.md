---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lansweeper.com
  spf: true
hosts:
- cert_expires: Sep 18 18:59:54 2026 GMT
  host: www.lansweeper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 09:03:52 2026 GMT
  host: developer.lansweeper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.lansweeper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lansweeper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lansweeper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lansweeper
provider_slug: lansweeper
slug: lansweeper-domain-security
source_filename: lansweeper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lansweeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:59:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lansweeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:03:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lansweeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lansweeper.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lansweeper/refs/heads/main/security/lansweeper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IT Asset Management
- Asset Discovery
- Cybersecurity Asset Management
- Network Discovery
- Software Asset Management
- GraphQL
---

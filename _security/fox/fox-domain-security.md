---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: foxcorporation.com
  spf: true
- caa:
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "certainly.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fox.com
  spf: true
hosts:
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: www.foxcorporation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 29 07:17:46 2026 GMT
  host: www.fox.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fox Corporation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fox Corporation
provider_slug: fox
slug: fox-domain-security
source_filename: fox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxcorporation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: false\n- host: www.fox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 07:17:46 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: foxcorporation.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fox.com\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox/refs/heads/main/security/fox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 500
- Media
- Broadcast
- News
- Sports
- Streaming
---

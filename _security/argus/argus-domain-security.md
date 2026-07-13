---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altusgroup.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: altusplatform.com
  spf: false
hosts:
- cert_expires: Sep  1 17:18:54 2026 GMT
  host: www.altusgroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:18:54 2026 GMT
  host: cloud.altusplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARGUS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ARGUS
provider_slug: argus
slug: argus-domain-security
source_filename: argus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altusgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.altusplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: altusgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: altusplatform.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argus/refs/heads/main/security/argus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Altus Group
- Asset Management
- Commercial Real Estate
- Fund Management
- Portfolio Management
- Real Estate Software
- Valuation
---

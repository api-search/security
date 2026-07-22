---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moonactive.com
  spf: true
hosts:
- cert_expires: Aug 30 03:01:45 2026 GMT
  host: www.moonactive.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moonactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoonActive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MoonActive
provider_slug: moonactive
slug: moonactive-domain-security
source_filename: moonactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moonactive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:01:45 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: moonactive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonactive/refs/heads/main/security/moonactive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Gaming
- Mobile Games
- Entertainment
- Casual Games
---

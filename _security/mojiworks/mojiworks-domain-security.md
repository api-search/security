---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mojiworks.com
  spf: true
hosts:
- cert_expires: Oct  4 02:14:49 2026 GMT
  host: www.mojiworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mojiworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mojiworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: mojiworks
provider_slug: mojiworks
slug: mojiworks-domain-security
source_filename: mojiworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mojiworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:14:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mojiworks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mojiworks/refs/heads/main/security/mojiworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Games
- Gaming
- Social Games
- Artificial Intelligence
- Generative AI
- Entertainment
- Consumer
---

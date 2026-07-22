---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: believer.gg
  spf: true
hosts:
- cert_expires: Sep 28 23:00:35 2026 GMT
  host: believer.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Believer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Believer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Believer
provider_slug: believer
slug: believer-domain-security
source_filename: believer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: believer.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:00:35 2026 GMT\n  hsts: false\ndomains:\n- domain: believer.gg\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/believer/refs/heads/main/security/believer-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Games
- Gaming
- Video Games
- Interactive Entertainment
- Game Development
- Los Angeles
---

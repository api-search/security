---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: inmemori.com
  spf: true
hosts:
- cert_expires: Sep 25 02:14:54 2026 GMT
  host: www.inmemori.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inmemori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inmemori, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Inmemori
provider_slug: inmemori
slug: inmemori-domain-security
source_filename: inmemori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inmemori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:14:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inmemori.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inmemori/refs/heads/main/security/inmemori-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Funeral Services
- End of Life
- Memorial
- France
- Ceremonies
---

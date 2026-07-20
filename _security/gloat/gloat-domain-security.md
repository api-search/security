---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gloat.com
  spf: true
hosts:
- cert_expires: Sep 14 21:09:54 2026 GMT
  host: www.gloat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gloat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gloat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gloat
provider_slug: gloat
slug: gloat-domain-security
source_filename: gloat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gloat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:09:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gloat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloat/refs/heads/main/security/gloat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Human Resources
- Talent Marketplace
- Skills
- Workforce
- Internal Mobility
- HR Tech
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: binadox.com
  spf: true
hosts:
- cert_expires: Aug 26 08:27:47 2026 GMT
  host: www.binadox.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binadox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binadox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Binadox
provider_slug: binadox
slug: binadox-domain-security
source_filename: binadox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.binadox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:27:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: binadox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binadox/refs/heads/main/security/binadox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SaaS Management
- Shadow IT
- Spend Optimization
- Cloud Cost
- License Management
- FinOps
- ITAM
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: verdantapp.com
  spf: true
hosts:
- cert_expires: Sep 13 01:43:49 2026 GMT
  host: www.verdantapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verdant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verdant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Verdant
provider_slug: verdant
slug: verdant-domain-security
source_filename: verdant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verdantapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: verdantapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdant/refs/heads/main/security/verdant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GovTech
- Permitting
- Local Government
- Land Use Planning
- Artificial Intelligence
- SaaS
---

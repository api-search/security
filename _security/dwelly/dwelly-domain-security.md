---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dwelly.group
  spf: true
hosts:
- cert_expires: Sep 29 04:40:03 2026 GMT
  host: www.dwelly.group
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dwelly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dwelly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dwelly
provider_slug: dwelly
slug: dwelly-domain-security
source_filename: dwelly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dwelly.group\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:40:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dwelly.group\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwelly/refs/heads/main/security/dwelly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Property Management
- Lettings
- PropTech
- Artificial Intelligence
- Automation
- United Kingdom
- Mergers and Acquisitions
---

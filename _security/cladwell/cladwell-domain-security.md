---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cladwell.com
  spf: true
hosts:
- cert_expires: Aug 20 04:58:13 2026 GMT
  host: cladwell.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cladwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cladwell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cladwell
provider_slug: cladwell
slug: cladwell-domain-security
source_filename: cladwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cladwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:58:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cladwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cladwell/refs/heads/main/security/cladwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- Wardrobe
- Sustainability
- Retail
- Consumer App
- AI Styling
---

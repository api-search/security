---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chaart.co
  spf: true
hosts:
- cert_expires: Sep  1 07:48:12 2026 GMT
  host: chaart.co
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chaart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chaart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chaart
provider_slug: chaart
slug: chaart-domain-security
source_filename: chaart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaart.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: chaart.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaart/refs/heads/main/security/chaart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Art
- Marketplace
- Collectibles
- Fintech
- Mobile App
- South Korea
- Consumer
---

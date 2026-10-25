---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sghl.com.au
  spf: true
hosts:
- cert_expires: Dec 12 11:54:54 2026 GMT
  host: sghl.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sghl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SGH Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SGH Ltd
provider_slug: sghl
slug: sghl-domain-security
source_filename: sghl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sghl.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 11:54:54 2026 GMT\n  hsts: false\ndomains:\n- domain: sghl.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sghl/refs/heads/main/security/sghl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Australia
- Industrial Services
- Energy
- Construction Materials
- Equipment Hire
- Media
- ASX Listed
---

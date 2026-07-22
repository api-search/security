---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: timberhub.com
  spf: true
hosts:
- cert_expires: Sep 27 02:56:52 2026 GMT
  host: www.timberhub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timberhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timberhub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Timberhub
provider_slug: timberhub
slug: timberhub-domain-security
source_filename: timberhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timberhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: timberhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timberhub/refs/heads/main/security/timberhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Timber
- Marketplace
- Supply Chain
- Sustainability
- EUDR Compliance
- B2B Trade
- Logistics
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: betterview.com
  spf: true
hosts:
- cert_expires: Aug  7 18:21:19 2026 GMT
  host: betterview.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betterview Marketplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetterView Marketplace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BetterView Marketplace
provider_slug: betterview-marketplace
slug: betterview-marketplace-domain-security
source_filename: betterview-marketplace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betterview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 18:21:19 2026 GMT\n  hsts: null\ndomains:\n- domain: betterview.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterview-marketplace/refs/heads/main/security/betterview-marketplace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Property Intelligence
- Insurance
- Insurtech
- Geospatial
- Underwriting
- Property Data
- Risk
---

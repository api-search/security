---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: art.com
  spf: true
hosts:
- cert_expires: Oct 29 02:45:16 2026 GMT
  host: www.art.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Art.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Art.com
provider_slug: artcom
slug: artcom-domain-security
source_filename: artcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.art.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 02:45:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: art.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artcom/refs/heads/main/security/artcom-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- E-commerce
- Art
- Retail
- Marketplace
- Online
---

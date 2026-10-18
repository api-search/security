---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: citiesocial.com
  spf: true
hosts:
- cert_expires: Dec  9 05:37:07 2026 GMT
  host: www.citiesocial.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citiesocial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citiesocial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Citiesocial
provider_slug: citiesocial
slug: citiesocial-domain-security
source_filename: citiesocial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citiesocial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 05:37:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\ndomains:\n- domain: citiesocial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citiesocial/refs/heads/main/security/citiesocial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Marketplace
- curated
- Taiwan
- Cross-Border
---

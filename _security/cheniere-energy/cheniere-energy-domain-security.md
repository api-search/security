---
api_specs:
- filename: cheniere.yml
  format: yaml
  label: Cheniere Energy Website
  slug: website
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cheniere.com
  spf: true
hosts:
- cert_expires: Sep 16 08:05:08 2026 GMT
  host: www.cheniere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cheniere Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cheniere Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cheniere Energy
provider_slug: cheniere-energy
slug: cheniere-energy-domain-security
source_filename: cheniere-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cheniere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:05:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cheniere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/security/cheniere-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corpus Christi
- Energy
- Export
- Houston
- LNG
- Liquefaction
- Natural Gas
- Regasification
- Sabine Pass
- Texas
---

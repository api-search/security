---
api_specs:
- filename: modo-energy-openapi.yml
  format: yaml
  label: Modo Energy
  slug: modo-energy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modo-energy/refs/heads/main/openapi/modo-energy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modoenergy.com
  spf: true
hosts:
- cert_expires: Oct  4 13:53:32 2026 GMT
  host: developers.modoenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.modoenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modo Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modo Energy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Modo Energy
provider_slug: modo-energy
slug: modo-energy-domain-security
source_filename: modo-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.modoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:53:32 2026 GMT\n  hsts: null\n- host: api.modoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: modoenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modo-energy/refs/heads/main/security/modo-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Battery Storage
- Utilities
- Data
---

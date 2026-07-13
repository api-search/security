---
api_specs:
- filename: arch-coal-investor-relations-api.yaml
  format: yaml
  label: Arch Coal Investor Relations
  slug: arch-coal-investor-relations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/openapi/arch-coal-investor-relations-api.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arch-coal.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: archresources.com
  spf: false
hosts:
- host: www.arch-coal.com
  https: false
- cert_expires: Jan 11 19:52:35 2027 GMT
  host: archresources.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.archresources.com
  https: false
kind: domain-security
layout: security
method: probed
name: Arch Coal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arch Coal, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Arch Coal
provider_slug: arch-coal
slug: arch-coal-domain-security
source_filename: arch-coal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arch-coal.com\n  https: false\n- host: archresources.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 19:52:35 2027 GMT\n  hsts: false\n- host: api.archresources.com\n  https: false\ndomains:\n- domain: arch-coal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: archresources.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/security/arch-coal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Fortune 500
---

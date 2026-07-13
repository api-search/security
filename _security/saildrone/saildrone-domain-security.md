---
api_specs:
- filename: saildrone-mission-api-openapi.yml
  format: yaml
  label: Saildrone Mission API
  slug: saildrone-mission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saildrone/refs/heads/main/openapi/saildrone-mission-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saildrone.com
  spf: true
hosts:
- cert_expires: Oct  2 07:58:33 2026 GMT
  host: www.saildrone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saildrone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saildrone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Saildrone
provider_slug: saildrone
slug: saildrone-domain-security
source_filename: saildrone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saildrone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:58:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: saildrone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saildrone/refs/heads/main/security/saildrone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maritime
- Ocean Data
- USV
- Unmanned Surface Vehicle
- Autonomous Systems
- METOC
- Maritime Domain Awareness
- Anti Submarine Warfare
- Defense
- Climate
- Oceanography
- Bathymetry
- Biogeochemical
---

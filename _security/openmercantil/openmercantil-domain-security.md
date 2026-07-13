---
api_specs:
- filename: openmercantil-openapi.yml
  format: yaml
  label: OpenMercantil Public API
  slug: openmercantil-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openmercantil.es
  spf: true
hosts:
- cert_expires: Oct  6 20:16:53 2026 GMT
  host: openmercantil.es
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openmercantil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenMercantil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenMercantil
provider_slug: openmercantil
slug: openmercantil-domain-security
source_filename: openmercantil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openmercantil.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:16:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openmercantil.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/security/openmercantil-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- Spain
- Company Data
- Business Registry
- BORME
- Public Records
- Spanish Companies
- CIF
- CNAE
- Public Procurement
- PLACSP
- CNMV
- OEPM
- BDNS
- OpenSanctions
- Public-Interest Data
- Spanish Open Data
- REST API
- JSON
- CSV
- Geocoding
- Trust Score
- Registry Timeline
- Daily Summary
---

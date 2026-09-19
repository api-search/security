---
api_specs:
- filename: es-pera-estado-api-openapi.yml
  format: yaml
  label: ES·pera API Estado API
  slug: es-pera-estado-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/openapi/es-pera-estado-api-openapi.yml
- filename: es-pera-hospitales-api-openapi.yml
  format: yaml
  label: ES·pera API Hospitales API
  slug: es-pera-hospitales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/openapi/es-pera-hospitales-api-openapi.yml
- filename: es-pera-listas-auton-micas-api-openapi.yml
  format: yaml
  label: ES·pera API Listas autonómicas API
  slug: es-pera-listas-auton-micas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/openapi/es-pera-listas-auton-micas-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: es-pera.org
  spf: true
hosts:
- cert_expires: Nov 20 09:55:55 2026 GMT
  host: es-pera.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Es Pera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ES·pera API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ES·pera API
provider_slug: es-pera
slug: es-pera-domain-security
source_filename: es-pera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: es-pera.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 09:55:55 2026 GMT\n  hsts: false\ndomains:\n- domain: es-pera.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/security/es-pera-domain-security.yml
summary_line: TLSv1.3
tags:
- Healthcare
- Open Data
- Waiting Lists
- hospital activity
- Spain
- Public Sector
- Government Data
- SNS
---

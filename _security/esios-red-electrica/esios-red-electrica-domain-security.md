---
api_specs:
- filename: esios-red-electrica-archives-api-openapi.yml
  format: yaml
  label: Red Electrica (e-sios) Archives API
  slug: esios-red-electrica-archives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esios-red-electrica/refs/heads/main/openapi/esios-red-electrica-archives-api-openapi.yml
- filename: esios-red-electrica-calculator-data-api-openapi.yml
  format: yaml
  label: Red Electrica (e-sios) Calculator Data API
  slug: esios-red-electrica-calculator-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esios-red-electrica/refs/heads/main/openapi/esios-red-electrica-calculator-data-api-openapi.yml
- filename: esios-red-electrica-contents-api-openapi.yml
  format: yaml
  label: Red Electrica (e-sios) Contents API
  slug: esios-red-electrica-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esios-red-electrica/refs/heads/main/openapi/esios-red-electrica-contents-api-openapi.yml
- filename: esios-red-electrica-es-api-openapi.yml
  format: yaml
  label: Red Electrica (e-sios) Es API
  slug: esios-red-electrica-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esios-red-electrica/refs/heads/main/openapi/esios-red-electrica-es-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ree.es
  spf: true
hosts:
- cert_expires: Dec 10 08:54:07 2026 GMT
  host: www.esios.ree.es
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Esios Red Electrica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Electrica (e-sios), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Red Electrica (e-sios)
provider_slug: esios-red-electrica
slug: esios-red-electrica-domain-security
source_filename: esios-red-electrica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esios.ree.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 08:54:07 2026 GMT\n  hsts: null\ndomains:\n- domain: ree.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esios-red-electrica/refs/heads/main/security/esios-red-electrica-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Data
- Spain
---

---
api_specs:
- filename: camara-openapi.yml
  format: yaml
  label: CAMARA Quality On Demand API
  slug: quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara/refs/heads/main/openapi/camara-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: camaraproject.org
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: camaraproject.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Camara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CAMARA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CAMARA
provider_slug: camara
slug: camara-domain-security
source_filename: camara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: camaraproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: camaraproject.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camara/refs/heads/main/security/camara-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Telecom
- Network APIs
- Standards
- Linux Foundation
- Open Gateway
- GSMA
- Connectivity
- 5G
---

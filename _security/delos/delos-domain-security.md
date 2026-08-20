---
api_specs:
- filename: delos-wellcube-cloud-be-openapi.yml
  format: yaml
  label: WellCube Cloud BE API
  slug: wellcube-cloud-be-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-wellcube-cloud-be-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: delos.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wellcube.io
  spf: false
hosts:
- cert_expires: Sep 21 08:02:09 2026 GMT
  host: delos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 06:33:48 2026 GMT
  host: wellcube.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: cloud.wellcube.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Delos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delos, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Delos
provider_slug: delos
slug: delos-domain-security
source_filename: delos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:02:09 2026 GMT\n  hsts: false\n- host: wellcube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 06:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.wellcube.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: delos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wellcube.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/security/delos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- wellness-real-estate
- Indoor Air Quality
- indoor-environmental-quality
- IoT
- Smart Buildings
- Building Automation
- Air Purification
- environmental-sensors
- Commercial Real Estate
- healthy-buildings
- Hospitality
- ESG
---

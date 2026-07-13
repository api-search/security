---
api_specs:
- filename: granular-farm-management-openapi.yml
  format: yaml
  label: Granular Farm Management API
  slug: granular-farm-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/openapi/granular-farm-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: granular.ag
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: granular.ag
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: api.granular.ag
  https: false
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: us.app.granular.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Granular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granular (Corteva Agriscience), probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Granular (Corteva Agriscience)
provider_slug: granular
slug: granular-domain-security
source_filename: granular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: granular.ag\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\n- host: api.granular.ag\n  https: false\n- host: us.app.granular.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: granular.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/security/granular-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Agriculture
- Farm Management
- Financial
- Crop Planning
- Agronomy
---

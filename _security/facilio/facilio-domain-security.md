---
api_specs:
- filename: facilio-openapi-original.yaml
  format: yaml
  label: Facilio REST API v5
  slug: facilio-rest-api-v5
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facilio/refs/heads/main/openapi/facilio-openapi-original.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: facilio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: facilioapis.com
  spf: false
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: facilio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: us.facilioapis.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Facilio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facilio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Facilio
provider_slug: facilio
slug: facilio-domain-security
source_filename: facilio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facilio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.facilioapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: facilio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: facilioapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facilio/refs/heads/main/security/facilio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Facility Management
- CMMS
- Property Operations
- Maintenance
- Asset Management
- Real Estate
- IoT
- Buildings
---

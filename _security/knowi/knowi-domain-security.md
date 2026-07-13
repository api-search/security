---
api_specs:
- filename: knowi-management-api-openapi.yml
  format: yaml
  label: Knowi Management API
  slug: knowi-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-management-api-openapi.yml
- filename: knowi-push-data-api-openapi.yml
  format: yaml
  label: Knowi Push Data API
  slug: knowi-push-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-push-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knowi.com
  spf: true
hosts:
- cert_expires: Mar 15 18:17:58 2027 GMT
  host: www.knowi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 18:17:58 2027 GMT
  host: knowi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knowi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knowi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knowi
provider_slug: knowi
slug: knowi-domain-security
source_filename: knowi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knowi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 18:17:58 2027 GMT\n  hsts: false\n- host: knowi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 18:17:58 2027 GMT\n  hsts: false\ndomains:\n- domain: knowi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/security/knowi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Analytics
- API Analytics
- Business Intelligence
- Data Visualization
- Embedded Analytics
- NoSQL Analytics
---

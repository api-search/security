---
api_specs:
- filename: americorps-openapi.yml
  format: yaml
  label: AmeriCorps Open Data SODA API
  slug: americorps-open-data-soda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/openapi/americorps-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: americorps.gov
  spf: true
hosts:
- cert_expires: Aug  6 23:59:59 2026 GMT
  host: americorps.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 13:23:10 2026 GMT
  host: data.americorps.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Americorps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AmeriCorps, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AmeriCorps
provider_slug: americorps
slug: americorps-domain-security
source_filename: americorps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: americorps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 23:59:59 2026 GMT\n  hsts: null\n- host: data.americorps.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 13:23:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: americorps.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/security/americorps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- National Service
- Volunteerism
- Community Development
- Civic Engagement
- Education
- Disaster Response
- Environmental Conservation
---

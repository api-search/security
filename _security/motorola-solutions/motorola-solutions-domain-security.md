---
api_specs:
- filename: motorola-solutions-motorola-api-openapi.yml
  format: yaml
  label: Motorola Solutions API
  slug: motorola-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motorola-solutions/refs/heads/main/openapi/motorola-solutions-motorola-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: motorolasolutions.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: developer.motorolasolutions.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 16 12:30:24 2026 GMT
  host: api.motorolasolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motorola Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motorola Solutions, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Motorola Solutions
provider_slug: motorola-solutions
slug: motorola-solutions-domain-security
source_filename: motorola-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.motorolasolutions.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.motorolasolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:30:24 2026 GMT\n  hsts: null\ndomains:\n- domain: motorolasolutions.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motorola-solutions/refs/heads/main/security/motorola-solutions-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Public Safety
- Communications
- Video Security
- IoT
- Fortune 500
---

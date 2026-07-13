---
api_specs:
- filename: apptio-openapi.yaml
  format: yaml
  label: Apptio API
  slug: apptio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptio/refs/heads/main/openapi/apptio-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: apptio.com
  spf: true
hosts:
- cert_expires: Aug 28 22:57:35 2026 GMT
  host: www.apptio.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- host: developer.apptio.com
  https: false
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.apptio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apptio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apptio, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Apptio
provider_slug: apptio
slug: apptio-domain-security
source_filename: apptio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apptio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:57:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.apptio.com\n  https: false\n- host: api.apptio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: apptio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptio/refs/heads/main/security/apptio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Cost Management
- IT Finance
- Technology Business Management
---

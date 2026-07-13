---
api_specs:
- filename: state-street-alpha-data-platform-openapi.yml
  format: yaml
  label: Alpha Data Platform API
  slug: alpha-data-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/openapi/state-street-alpha-data-platform-openapi.yml
- filename: state-street-fund-connect-openapi.yml
  format: yaml
  label: Fund Connect API
  slug: fund-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/openapi/state-street-fund-connect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: statestreet.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.statestreet.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: developer.statestreet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.statestreet.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: State Street Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for State Street, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: State Street
provider_slug: state-street
slug: state-street-domain-security
source_filename: state-street-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.statestreet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.statestreet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.statestreet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: statestreet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/security/state-street-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---

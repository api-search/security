---
api_specs:
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Authentication API
  slug: tributetech-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Serving Locations API
  slug: tributetech-serving-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Obituaries API
  slug: tributetech-obituaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tributetech.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tributecenteronline.com
  spf: true
hosts:
- cert_expires: Sep  6 00:55:28 2026 GMT
  host: www.tributetech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.tributecenteronline.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.demo.tributecenteronline.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tributetech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tribute Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tribute Technology
provider_slug: tributetech
slug: tributetech-domain-security
source_filename: tributetech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tributetech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:55:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tributecenteronline.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\n- host: api.demo.tributecenteronline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tributetech.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tributecenteronline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/security/tributetech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Funeral Technology
- Obituaries
- Memorials
- Funeral Homes
- E-commerce
- Death Care
- Case Management
---

---
api_specs:
- filename: apptimize-rest-api-openapi.yml
  format: yaml
  label: Apptimize REST API
  slug: apptimize-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptimize/refs/heads/main/openapi/apptimize-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apptimize.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: apptimize.eu
  spf: true
hosts:
- cert_expires: Oct  5 10:57:33 2026 GMT
  host: apptimize.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 10:57:33 2026 GMT
  host: api.apptimize.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 02:09:39 2026 GMT
  host: api.apptimize.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apptimize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apptimize, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apptimize
provider_slug: apptimize
slug: apptimize-domain-security
source_filename: apptimize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apptimize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:57:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.apptimize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:57:33 2026 GMT\n  hsts: null\n- host: api.apptimize.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:09:39 2026 GMT\n  hsts: null\ndomains:\n- domain: apptimize.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apptimize.eu\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptimize/refs/heads/main/security/apptimize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- A/B Testing
- Feature Flags
- Feature Management
- Experimentation
- Mobile
- SDK
- Optimization
---

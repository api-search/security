---
api_specs:
- filename: aspentech-inmation-web-openapi.yml
  format: yaml
  label: AspenTech Inmation Web API
  slug: inmation-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/openapi/aspentech-inmation-web-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aspentech.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inmation.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.aspentech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 08:30:25 2026 GMT
  host: dev.knowledgecenter.aspentech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 21:21:29 2026 GMT
  host: atdocs.inmation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aspentech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AspenTech, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AspenTech
provider_slug: aspentech
slug: aspentech-domain-security
source_filename: aspentech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aspentech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.knowledgecenter.aspentech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:30:25 2026 GMT\n  hsts: null\n- host: atdocs.inmation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 21:21:29 2026 GMT\n  hsts: false\ndomains:\n- domain: aspentech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: inmation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/security/aspentech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial IoT
- Process Optimization
- Manufacturing
- Energy
- Chemicals
- Time Series
---

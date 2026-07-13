---
api_specs:
- filename: axway-amplify-platform-openapi-original.json
  format: json
  label: Axway Amplify Platform API
  slug: axway-amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/openapi/axway-amplify-platform-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axway.com
  spf: true
hosts:
- host: developer.axway.com
  https: false
- cert_expires: Sep 26 11:35:30 2026 GMT
  host: www.axway.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: platform.axway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axway, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axway
provider_slug: axway
slug: axway-domain-security
source_filename: axway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.axway.com\n  https: false\n- host: www.axway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:35:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: platform.axway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axway/refs/heads/main/security/axway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- Enterprise
- Integration
- Security
---

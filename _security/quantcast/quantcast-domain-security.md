---
api_specs:
- filename: QuantcastDeveloperAPI.postman_collection.json
  format: json
  label: Quantcast Platform GraphQL API
  slug: quantcast-platform-graphql-api
  spec_type: Postman
  url: https://developers.quantcast.com/docs/QuantcastDeveloperAPI.postman_collection.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:netsec-notifications@quantcast.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quantcast.com
  spf: true
hosts:
- cert_expires: Oct 25 06:28:41 2026 GMT
  host: www.quantcast.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 06:28:41 2026 GMT
  host: developers.quantcast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 13:12:42 2026 GMT
  host: help.quantcast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantcast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quantcast
provider_slug: quantcast
slug: quantcast-domain-security
source_filename: quantcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quantcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 06:28:41 2026 GMT\n  hsts: false\n- host: developers.quantcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 06:28:41 2026 GMT\n  hsts: null\n- host: help.quantcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quantcast.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:netsec-notifications@quantcast.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantcast/refs/heads/main/security/quantcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AdTech
- Programmatic Advertising
- Demand-Side Platform
- DSP
- Audience Measurement
- Audience Intelligence
- Consent Management
- CMP
- Privacy
- GraphQL
- Conversion Tracking
- CTV
- Video Advertising
- Display Advertising
- Artificial Intelligence
- Audience Graph
---

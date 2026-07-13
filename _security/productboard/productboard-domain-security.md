---
api_specs:
- filename: productboard-openapi.yml
  format: yaml
  label: Productboard Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productboard/refs/heads/main/openapi/productboard-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:infrastructure@productboard.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: productboard.com
  spf: true
hosts:
- cert_expires: Aug 28 00:14:27 2026 GMT
  host: www.productboard.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 00:46:46 2026 GMT
  host: developer.productboard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 06:47:32 2026 GMT
  host: api.productboard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Productboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Productboard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Productboard
provider_slug: productboard
slug: productboard-domain-security
source_filename: productboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.productboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:14:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.productboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.productboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 06:47:32 2026 GMT\n  hsts: null\ndomains:\n- domain: productboard.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:infrastructure@productboard.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productboard/refs/heads/main/security/productboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Product Management
- Roadmapping
- Customer Feedback
- Prioritization
- Product Operations
---

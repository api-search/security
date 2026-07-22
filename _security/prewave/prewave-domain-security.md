---
api_specs:
- filename: prewave-openapi-original.json
  format: json
  label: Public Prewave API
  slug: public-prewave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prewave/refs/heads/main/openapi/prewave-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: prewave.com
  spf: true
hosts:
- cert_expires: Oct  7 11:16:11 2026 GMT
  host: www.prewave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prewave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prewave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Prewave
provider_slug: prewave
slug: prewave-domain-security
source_filename: prewave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prewave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:16:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prewave.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prewave/refs/heads/main/security/prewave-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Saas
- Supply Chain
- Risk Intelligence
- Sustainability
- Compliance
- EUDR
- Supplier Management
---

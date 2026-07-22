---
api_specs:
- filename: whoapi-openapi.yml
  format: yaml
  label: WhoAPI Domain Intelligence API
  slug: whoapi-domain-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoapi/refs/heads/main/openapi/whoapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: whoapi.com
  spf: true
hosts:
- cert_expires: Aug 28 14:14:02 2026 GMT
  host: whoapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 04:55:46 2026 GMT
  host: api.whoapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whoapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WhoAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WhoAPI
provider_slug: whoapi
slug: whoapi-domain-security
source_filename: whoapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whoapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 14:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.whoapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:55:46 2026 GMT\n  hsts: null\ndomains:\n- domain: whoapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoapi/refs/heads/main/security/whoapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Domains
- WHOIS
- Domain Availability
- SSL
- Email Verification
- Blacklist
- Cybersecurity
- Domain Intelligence
- Screenshots
- Reputation
---

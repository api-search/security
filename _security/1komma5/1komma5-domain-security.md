---
api_specs:
- filename: 1komma5-offer-tool-openapi-original.json
  format: json
  label: 1KOMMA5° Offer Tool API
  slug: 1komma5-offer-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1komma5/refs/heads/main/openapi/1komma5-offer-tool-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 1komma5.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 1komma5grad.com
  spf: true
hosts:
- cert_expires: Oct  2 18:13:57 2026 GMT
  host: 1komma5.com
  hsts: true
  hsts_max_age: 31104000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 20:27:16 2026 GMT
  host: api.offer.1komma5grad.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:46:06 2026 GMT
  host: help.1komma5.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: heartbeat.1komma5grad.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: auth.1komma5grad.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Komma5 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1KOMMA5°, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 1KOMMA5°
provider_slug: 1komma5
slug: 1komma5-domain-security
source_filename: 1komma5-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1komma5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:13:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31104000\n- host: api.offer.1komma5grad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:27:16 2026 GMT\n  hsts: false\n- host: help.1komma5.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:46:06 2026 GMT\n  hsts: false\n- host: heartbeat.1komma5grad.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n- host: auth.1komma5grad.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: 1komma5.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: 1komma5grad.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1komma5/refs/heads/main/security/1komma5-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Solar
- Renewable Energy
- Smart Home
- Electric Vehicles
- Heat Pumps
- Virtual Power Plant
- Energy Management
- Germany
---

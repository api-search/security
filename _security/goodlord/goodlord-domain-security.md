---
api_specs:
- filename: goodlord-referencing-api-openapi.json
  format: json
  label: Goodlord Referencing API
  slug: goodlord-referencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-referencing-api-openapi.json
- filename: goodlord-referencing-api-sandbox-openapi.json
  format: json
  label: Goodlord Referencing API (Sandbox)
  slug: goodlord-referencing-api-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-referencing-api-sandbox-openapi.json
- filename: goodlord-insurance-app-api-openapi.json
  format: json
  label: Goodlord Insurance App API
  slug: goodlord-insurance-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-insurance-app-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodlord.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodlord.co
  spf: true
hosts:
- cert_expires: Oct  2 13:41:03 2026 GMT
  host: www.goodlord.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 06:46:24 2026 GMT
  host: portal.goodlord.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.goodoverlord.com
  https: false
kind: domain-security
layout: security
method: probed
name: Goodlord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodlord, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Goodlord
provider_slug: goodlord
slug: goodlord-domain-security
source_filename: goodlord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodlord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:41:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.goodlord.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:46:24 2026 GMT\n  hsts: false\n- host: api.goodoverlord.com\n  https: false\ndomains:\n- domain: goodlord.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: goodlord.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/security/goodlord-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United Kingdom
- PropTech
- Property Management
- Rentals
- Lettings
- Tenant Referencing
- Tenancy Management
- Insurance
- Payments
---

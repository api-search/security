---
api_specs:
- filename: canopy-openapi.json
  format: json
  label: Canopy Connect API
  slug: canopy-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/openapi/canopy-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: usecanopy.com
  spf: true
hosts:
- cert_expires: Nov 30 16:02:52 2026 GMT
  host: www.usecanopy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: app.usecanopy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Canopy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canopy Connect, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Canopy Connect
provider_slug: canopy
slug: canopy-domain-security
source_filename: canopy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usecanopy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 16:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.usecanopy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usecanopy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/security/canopy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Auto Insurance
- Casualty
- Financial-Services
- Homeowners Insurance
- Insurance
- Insurance Verification
- Property
---

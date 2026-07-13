---
api_specs:
- filename: didomi-platform-api-openapi.yml
  format: yaml
  label: Didomi Platform API
  slug: didomi-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didomi/refs/heads/main/openapi/didomi-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: didomi.io
  spf: true
hosts:
- cert_expires: Sep 11 12:57:14 2026 GMT
  host: www.didomi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 14:30:52 2026 GMT
  host: developers.didomi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.didomi.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Didomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Didomi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Didomi
provider_slug: didomi
slug: didomi-domain-security
source_filename: didomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.didomi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:57:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.didomi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.didomi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: didomi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didomi/refs/heads/main/security/didomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AdTech
- CCPA
- CMP
- Consent
- Consent Management
- DSAR
- Data Privacy
- GDPR
- IAB TCF
- MarTech
- Preference Management
- Privacy
- Privacy Requests
- Regulatory Compliance
---

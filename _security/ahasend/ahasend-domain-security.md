---
api_specs:
- filename: ahasend-openapi.yml
  format: yaml
  label: AhaSend
  slug: ahasend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ahasend.com
  spf: true
hosts:
- cert_expires: Aug 19 15:55:34 2026 GMT
  host: ahasend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 09:30:23 2026 GMT
  host: api.ahasend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ahasend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AhaSend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AhaSend
provider_slug: ahasend
slug: ahasend-domain-security
source_filename: ahasend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ahasend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:55:34 2026 GMT\n  hsts: false\n- host: api.ahasend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 09:30:23 2026 GMT\n  hsts: null\ndomains:\n- domain: ahasend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/security/ahasend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
---

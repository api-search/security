---
api_specs:
- filename: fathom-analytics-api-openapi.yml
  format: yaml
  label: Fathom Analytics REST API
  slug: fathom-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fathom/refs/heads/main/openapi/fathom-analytics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usefathom.com
  spf: true
hosts:
- cert_expires: Sep 19 00:23:16 2026 GMT
  host: usefathom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.usefathom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fathom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fathom Analytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fathom Analytics
provider_slug: fathom
slug: fathom-domain-security
source_filename: fathom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usefathom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 00:23:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.usefathom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: usefathom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fathom/refs/heads/main/security/fathom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Privacy
- GDPR
- Website Analytics
- Cookieless
- Page Views
- Events
- Reporting
---

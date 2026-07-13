---
api_specs:
- filename: usergems-api-openapi.yml
  format: yaml
  label: UserGems API
  slug: usergems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usergems.com
  spf: true
hosts:
- cert_expires: Aug 17 09:40:57 2026 GMT
  host: www.usergems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: app.usergems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.usergems.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usergems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UserGems, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UserGems
provider_slug: usergems
slug: usergems-domain-security
source_filename: usergems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usergems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 09:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.usergems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usergems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usergems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/security/usergems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Intelligence
- Outbound
- ABM
- Champion Tracking
- Job Changes
- Buying Signals
- AI Scoring
- Sales Engagement
- CRM
- Revenue Operations
- GTM
---

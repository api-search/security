---
api_specs:
- filename: snappr-openapi.yml
  format: yaml
  label: Snappr API
  slug: snappr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snappr.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: snappr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 08:28:50 2026 GMT
  host: docs.snappr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: api.snappr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snappr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snappr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Snappr
provider_slug: snappr
slug: snappr-domain-security
source_filename: snappr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snappr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: false\n- host: docs.snappr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:28:50 2026 GMT\n  hsts: false\n- host: api.snappr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: snappr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/security/snappr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Photography
- Videography
- Visual Content
- Photo Editing
- On-Demand
- Enterprise
---

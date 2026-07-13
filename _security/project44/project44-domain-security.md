---
api_specs:
- filename: project44-tracking-openapi.yml
  format: yaml
  label: project44 API v4
  slug: project44-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/openapi/project44-tracking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: project44.com
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.project44.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:25:38 2026 GMT
  host: developers.project44.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 29 11:00:45 2026 GMT
  host: na12.api.project44.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Project44 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for project44, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: project44
provider_slug: project44
slug: project44-domain-security
source_filename: project44-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.project44.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.project44.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:25:38 2026 GMT\n  hsts: false\n- host: na12.api.project44.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 11:00:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: project44.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/security/project44-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Supply Chain Visibility
- Tracking
- Freight
- Multi-modal
---

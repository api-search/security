---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Canto REST API
  slug: canto-rest-api
  spec_type: OpenAPI
  url: https://canto1.portal.swaggerhub.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: canto.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.canto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 16:25:40 2026 GMT
  host: api.canto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Canto
provider_slug: canto
slug: canto-domain-security
source_filename: canto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.canto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:25:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/security/canto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Asset Management
- DAM
- Brand Assets
- Images
- Videos
- Documents
- Media Library
- Asset Distribution
---

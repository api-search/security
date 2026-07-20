---
api_specs:
- filename: clearslide-openapi.yml
  format: yaml
  label: ClearSlide Platform API
  slug: clearslide-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clearslide.com
  spf: true
hosts:
- cert_expires: Sep 23 04:02:50 2026 GMT
  host: developer.clearslide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: platform.clearslide.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clearslide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearSlide, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ClearSlide
provider_slug: clearslide
slug: clearslide-domain-security
source_filename: clearslide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.clearslide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:02:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.clearslide.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: clearslide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/security/clearslide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales Engagement
- Sales Enablement
- Content Management
- Presentations
- Analytics
- Meetings
- CRM
- OAuth
- SCIM
---

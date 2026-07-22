---
api_specs:
- filename: templafy-public-api-v3-openapi.json
  format: json
  label: Templafy Public API
  slug: templafy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-public-api-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: templafy.com
  spf: true
hosts:
- cert_expires: Sep 14 19:50:53 2026 GMT
  host: www.templafy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Templafy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Templafy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Templafy
provider_slug: templafy
slug: templafy-domain-security
source_filename: templafy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.templafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:50:53 2026 GMT\n  hsts: false\ndomains:\n- domain: templafy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/security/templafy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Document Generation
- Templates
- Content Management
- Digital Asset Management
- Document Automation
- Productivity
- Enterprise
- SaaS
---

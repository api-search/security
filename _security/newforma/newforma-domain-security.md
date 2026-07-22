---
api_specs:
- filename: newforma-konekt-openapi-original.json
  format: json
  label: Newforma Konekt REST API
  slug: newforma-konekt-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newforma/refs/heads/main/openapi/newforma-konekt-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bimtrackapp.co
  spf: true
hosts:
- cert_expires: Dec 28 17:49:02 2026 GMT
  host: api.bimtrackapp.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newforma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newforma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Newforma
provider_slug: newforma
slug: newforma-domain-security
source_filename: newforma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.bimtrackapp.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 17:49:02 2026 GMT\n  hsts: null\ndomains:\n- domain: bimtrackapp.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newforma/refs/heads/main/security/newforma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AEC
- Construction
- Architecture
- Engineering
- BIM
- Building Information Modeling
- Project Management
- Issue Tracking
- Collaboration
---

---
api_specs:
- filename: cintoo-openapi-original.json
  format: json
  label: Cintoo Open API
  slug: cintoo-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cintoo/refs/heads/main/openapi/cintoo-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cintoo.com
  spf: true
hosts:
- cert_expires: Sep 15 07:30:45 2026 GMT
  host: aec.cintoo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cintoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cintoo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cintoo
provider_slug: cintoo
slug: cintoo-domain-security
source_filename: cintoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aec.cintoo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:30:45 2026 GMT\n  hsts: false\ndomains:\n- domain: cintoo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cintoo/refs/heads/main/security/cintoo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure SaaS
- Reality Capture
- Digital Twin
- Point Cloud
- 3D
- AEC
- BIM
- Construction
- Scan-to-BIM
- GIS
---

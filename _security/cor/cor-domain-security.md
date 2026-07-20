---
api_specs:
- filename: cor-openapi.json
  format: json
  label: COR API
  slug: cor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cor/refs/heads/main/openapi/cor-openapi.json
- filename: cor-resource-allocation-openapi.json
  format: json
  label: COR Resource Allocation API
  slug: cor-resource-allocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cor/refs/heads/main/openapi/cor-resource-allocation-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: projectcor.com
  spf: true
hosts:
- cert_expires: Sep 29 13:38:49 2026 GMT
  host: projectcor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api.projectcor.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: planner.svc.v2.projectcor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: COR
provider_slug: cor
slug: cor-domain-security
source_filename: cor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: projectcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:38:49 2026 GMT\n  hsts: false\n- host: api.projectcor.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: false\n- host: planner.svc.v2.projectcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: projectcor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cor/refs/heads/main/security/cor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agency Management
- Project Management
- Time Tracking
- Profitability
- Resource Allocation
- Professional Services
- MCP
---

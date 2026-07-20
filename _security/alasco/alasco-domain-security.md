---
api_specs:
- filename: alasco-fincon-openapi.json
  format: json
  label: Alasco FinCon API
  slug: alasco-fincon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-fincon-openapi.json
- filename: alasco-capex-openapi.json
  format: json
  label: Alasco CapEx API
  slug: alasco-capex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-capex-openapi.json
- filename: alasco-esg-openapi.json
  format: json
  label: Alasco ESG API
  slug: alasco-esg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-esg-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alasco.de
  spf: true
hosts:
- cert_expires: Oct  5 14:25:43 2026 GMT
  host: www.alasco.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 04:56:52 2026 GMT
  host: api.alasco.de
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alasco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alasco, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alasco
provider_slug: alasco
slug: alasco-domain-security
source_filename: alasco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alasco.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:25:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alasco.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:56:52 2026 GMT\n  hsts: null\ndomains:\n- domain: alasco.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/security/alasco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Real Estate
- Construction
- PropTech
- Financial Management
- Cost Management
- Capital Expenditure
- ESG
- Sustainability
---

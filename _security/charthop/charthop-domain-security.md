---
api_specs:
- filename: charthop-openapi-original.json
  format: json
  label: ChartHop REST API
  slug: charthop-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charthop/refs/heads/main/openapi/charthop-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charthop.com
  spf: true
hosts:
- cert_expires: Sep 28 07:34:11 2026 GMT
  host: www.charthop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charthop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charthop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Charthop
provider_slug: charthop
slug: charthop-domain-security
source_filename: charthop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charthop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:34:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: charthop.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charthop/refs/heads/main/security/charthop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HR
- People Analytics
- HRIS
- Workforce Planning
- Compensation
- Human Resources
- Org Chart
- MCP
---

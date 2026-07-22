---
api_specs:
- filename: xiaoman-openapi.yml
  format: yaml
  label: Xiaoman OKKI CRM Open API
  slug: xiaoman-okki-crm-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-openapi.yml
- filename: xiaoman-okki-go-openapi.yml
  format: yaml
  label: OKKI Go API
  slug: okki-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-okki-go-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xiaoman.cn
  spf: true
hosts:
- cert_expires: Dec 14 04:53:00 2026 GMT
  host: xiaoman.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 14 04:53:00 2026 GMT
  host: api-sandbox.xiaoman.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xiaoman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xiaoman (OKKI), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Xiaoman (OKKI)
provider_slug: xiaoman
slug: xiaoman-domain-security
source_filename: xiaoman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xiaoman.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 04:53:00 2026 GMT\n  hsts: false\n- host: api-sandbox.xiaoman.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 04:53:00 2026 GMT\n  hsts: false\ndomains:\n- domain: xiaoman.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/security/xiaoman-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- CRM
- Foreign Trade
- B2B
- Sales
- Prospecting
- Email Marketing
- AI Agents
- China
- Alibaba
---

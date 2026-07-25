---
api_specs:
- filename: xiaoman-companies-api-openapi.yml
  format: yaml
  label: Xiaoman (OKKI) Companies API
  slug: xiaoman-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-companies-api-openapi.yml
- filename: xiaoman-contacts-api-openapi.yml
  format: yaml
  label: Xiaoman (OKKI) Contacts API
  slug: xiaoman-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-contacts-api-openapi.yml
- filename: xiaoman-credits-api-openapi.yml
  format: yaml
  label: Xiaoman (OKKI) Credits API
  slug: xiaoman-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-credits-api-openapi.yml
- filename: xiaoman-default-api-openapi.yml
  format: yaml
  label: Xiaoman (OKKI) 产品 API
  slug: xiaoman-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-default-api-openapi.yml
- filename: xiaoman-devops-api-openapi.yml
  format: yaml
  label: Xiaoman (OKKI) devops相关 API
  slug: xiaoman-devops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-devops-api-openapi.yml
- filename: xiaoman-emails-api-openapi.yml
  format: yaml
  label: Xiaoman (OKKI) Emails API
  slug: xiaoman-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-emails-api-openapi.yml
- filename: xiaoman-s7-1-api-openapi.yml
  format: yaml
  label: Xiaoman (OKKI) s7.1 API
  slug: xiaoman-s7-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xiaoman/refs/heads/main/openapi/xiaoman-s7-1-api-openapi.yml
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

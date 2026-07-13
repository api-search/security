---
api_specs:
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Management API
  slug: encompass-loan-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Pipeline API
  slug: encompass-loan-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Borrower Pair & Applications API
  slug: encompass-borrower-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Contacts API
  slug: encompass-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass eFolder Documents & Attachments API
  slug: encompass-efolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Milestones & Associates API
  slug: encompass-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Conditions API
  slug: encompass-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Users API
  slug: encompass-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Webhooks API
  slug: encompass-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icemortgagetechnology.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elliemae.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.icemortgagetechnology.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:25:55 2026 GMT
  host: developer.icemortgagetechnology.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api.elliemae.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Encompass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encompass, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Encompass
provider_slug: encompass
slug: encompass-domain-security
source_filename: encompass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icemortgagetechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: developer.icemortgagetechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:25:55 2026 GMT\n  hsts: null\n- host: api.elliemae.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: icemortgagetechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: elliemae.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/security/encompass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mortgage
- Loan Origination
- LOS
- Fintech
- ICE Mortgage Technology
- Ellie Mae
- Lending
---

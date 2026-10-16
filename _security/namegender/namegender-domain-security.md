---
api_specs:
- filename: namegender-account-api-openapi.yml
  format: yaml
  label: NameGender Account API
  slug: namegender-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namegender/refs/heads/main/openapi/namegender-account-api-openapi.yml
- filename: namegender-batches-api-openapi.yml
  format: yaml
  label: NameGender Batches API
  slug: namegender-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namegender/refs/heads/main/openapi/namegender-batches-api-openapi.yml
- filename: namegender-gender-api-openapi.yml
  format: yaml
  label: NameGender Gender API
  slug: namegender-gender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namegender/refs/heads/main/openapi/namegender-gender-api-openapi.yml
- filename: namegender-webhooks-api-openapi.yml
  format: yaml
  label: NameGender Webhooks API
  slug: namegender-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namegender/refs/heads/main/openapi/namegender-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: namegender.com
  spf: true
hosts:
- cert_expires: Nov 25 05:30:20 2026 GMT
  host: namegender.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Namegender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NameGender, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NameGender
provider_slug: namegender
slug: namegender-domain-security
source_filename: namegender-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namegender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 05:30:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: namegender.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namegender/refs/heads/main/security/namegender-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gender
- Names
- Data Enrichment
- API
- Demographics
- Bulk
---

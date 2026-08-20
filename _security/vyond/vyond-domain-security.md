---
api_specs:
- filename: vyond-content-generation-api-openapi.yml
  format: yaml
  label: Vyond Content Generation API
  slug: vyond-content-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-content-generation-api-openapi.yml
- filename: vyond-parameter-api-openapi.yml
  format: yaml
  label: Vyond Parameter API
  slug: vyond-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-parameter-api-openapi.yml
- filename: vyond-scim-api-openapi.yml
  format: yaml
  label: Vyond SCIM API
  slug: vyond-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-scim-api-openapi.yml
- filename: vyond-turbo-api-openapi.yml
  format: yaml
  label: Vyond Turbo API
  slug: vyond-turbo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-turbo-api-openapi.yml
- filename: vyond-user-api-openapi.yml
  format: yaml
  label: Vyond User API
  slug: vyond-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-user-api-openapi.yml
- filename: vyond-video-api-openapi.yml
  format: yaml
  label: Vyond Video API
  slug: vyond-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-video-api-openapi.yml
- filename: vyond-video-export-api-openapi.yml
  format: yaml
  label: Vyond Video Export API
  slug: vyond-video-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-video-export-api-openapi.yml
- filename: vyond-webhook-api-openapi.yml
  format: yaml
  label: Vyond Webhook API
  slug: vyond-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vyond.com
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.vyond.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: api.vyond.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vyond Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vyond, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vyond
provider_slug: vyond
slug: vyond-domain-security
source_filename: vyond-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vyond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vyond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vyond.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/security/vyond-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Animation
- Video Generation
- Artificial Intelligence
- E-Learning
- Learning and Development
- Content Generation
- SCIM
- Identity Provisioning
- Webhook
- Enterprise
- Media
---

---
api_specs:
- filename: sanity-openapi.yml
  format: yaml
  label: Sanity Query API
  slug: sanity-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/openapi/sanity-openapi.yml
- filename: sanity-webhooks-asyncapi.yml
  format: yaml
  label: Sanity Webhooks API
  slug: sanity-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/asyncapi/sanity-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sanity.io
  spf: true
hosts:
- cert_expires: Sep 12 11:00:52 2026 GMT
  host: www.sanity.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sanity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sanity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sanity
provider_slug: sanity
slug: sanity-domain-security
source_filename: sanity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sanity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:00:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sanity.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/security/sanity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Headless CMS
- Content Management
- GROQ
- Real-Time
- Structured Content
- Developer Platform
---

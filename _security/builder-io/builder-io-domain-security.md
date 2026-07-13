---
api_specs:
- filename: builder-io-content-api-openapi.yml
  format: yaml
  label: Builder.io Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builder-io/refs/heads/main/openapi/builder-io-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: builder.io
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.builder.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: cdn.builder.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Builder Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Builder.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Builder.io
provider_slug: builder-io
slug: builder-io-domain-security
source_filename: builder-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.builder.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n- host: cdn.builder.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: builder.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builder-io/refs/heads/main/security/builder-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Headless CMS
- Visual Development
- Content Delivery
- A/B Testing
- GraphQL
- REST
- Personalization
- Page Building
---

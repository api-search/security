---
api_specs:
- filename: overview
  format: yaml
  label: KeystoneJS GraphQL API
  slug: keystonejs-graphql-api
  spec_type: OpenAPI
  url: https://keystonejs.com/docs/graphql/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keystonejs.com
  spf: true
hosts:
- cert_expires: Sep 24 08:45:44 2026 GMT
  host: keystonejs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keystonejs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeystoneJS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KeystoneJS
provider_slug: keystonejs
slug: keystonejs-domain-security
source_filename: keystonejs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keystonejs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:45:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: keystonejs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keystonejs/refs/heads/main/security/keystonejs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Headless CMS
- GraphQL
- Node.js
- Content Management
- Open Source
- TypeScript
- Prisma
---

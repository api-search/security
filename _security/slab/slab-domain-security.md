---
api_specs:
- filename: slab-openapi.yml
  format: yaml
  label: Slab Posts
  slug: posts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
- filename: slab-openapi.yml
  format: yaml
  label: Slab Topics
  slug: topics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
- filename: slab-openapi.yml
  format: yaml
  label: Slab Users
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
- filename: slab-openapi.yml
  format: yaml
  label: Slab Organization
  slug: organization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/openapi/slab-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slab.com
  spf: true
hosts:
- cert_expires: Sep 15 04:00:33 2026 GMT
  host: slab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:28 2026 GMT
  host: help.slab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:28 2026 GMT
  host: api.slab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slab, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slab
provider_slug: slab
slug: slab-domain-security
source_filename: slab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:00:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.slab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.slab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: slab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slab/refs/heads/main/security/slab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Base
- Wiki
- Documentation
- Collaboration
- GraphQL
---

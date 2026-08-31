---
api_specs:
- filename: permutive-contextual-api-openapi.yml
  format: yaml
  label: Permutive Contextual API
  slug: permutive-contextual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-contextual-api-openapi.yml
- filename: permutive-api-version-1-api-openapi.yml
  format: yaml
  label: Permutive API version 1 API
  slug: permutive-api-version-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-api-version-1-api-openapi.yml
- filename: permutive-v1-api-openapi.yml
  format: yaml
  label: Permutive V1 API
  slug: permutive-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-v1-api-openapi.yml
- filename: permutive-v2-0-api-openapi.yml
  format: yaml
  label: Permutive V2.0 API
  slug: permutive-v2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-v2-0-api-openapi.yml
- filename: permutive-v2-api-openapi.yml
  format: yaml
  label: Permutive V2 API
  slug: permutive-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: permutive.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: permutive.app
  spf: false
hosts:
- cert_expires: Oct 23 13:47:47 2026 GMT
  host: permutive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 19:08:20 2026 GMT
  host: docs.permutive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 03:15:31 2026 GMT
  host: api.permutive.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Permutive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Permutive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Permutive
provider_slug: permutive
slug: permutive-domain-security
source_filename: permutive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: permutive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 13:47:47 2026 GMT\n  hsts: false\n- host: docs.permutive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.permutive.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:15:31 2026 GMT\n  hsts: null\ndomains:\n- domain: permutive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: permutive.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/security/permutive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Publishing
- Advertising
- AdTech
- MarTech
- Audience
- Data Collaboration
- Data Management Platform
- Contextual
- Identity
- Segmentation
- Agents
---

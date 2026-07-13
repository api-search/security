---
api_specs:
- filename: hypertune-openapi.yml
  format: yaml
  label: Hypertune Flag Evaluation / Config (GraphQL / SDK) API
  slug: hypertune-flag-evaluation-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/openapi/hypertune-openapi.yml
- filename: hypertune-openapi.yml
  format: yaml
  label: Hypertune Edge Config Delivery API
  slug: hypertune-edge-config-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/openapi/hypertune-openapi.yml
- filename: hypertune-openapi.yml
  format: yaml
  label: Hypertune Analytics / Events API
  slug: hypertune-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/openapi/hypertune-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hypertune.com
  spf: true
hosts:
- cert_expires: Oct  1 07:05:48 2026 GMT
  host: www.hypertune.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:12:31 2026 GMT
  host: docs.hypertune.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 13:03:13 2026 GMT
  host: edge.hypertune.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hypertune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hypertune, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hypertune
provider_slug: hypertune
slug: hypertune-domain-security
source_filename: hypertune-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hypertune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:05:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hypertune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:12:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: edge.hypertune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:03:13 2026 GMT\n  hsts: null\ndomains:\n- domain: hypertune.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypertune/refs/heads/main/security/hypertune-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Feature Flags
- Experimentation
- A/B Testing
- Analytics
- App Configuration
- GraphQL
- Edge
---

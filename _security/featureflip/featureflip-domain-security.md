---
api_specs:
- filename: featureflip-client-sdk-api-openapi.yml
  format: yaml
  label: Featureflip Client SDK API
  slug: featureflip-client-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-client-sdk-api-openapi.yml
- filename: featureflip-environments-api-openapi.yml
  format: yaml
  label: Featureflip Environments API
  slug: featureflip-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-environments-api-openapi.yml
- filename: featureflip-feature-flags-api-openapi.yml
  format: yaml
  label: Featureflip Feature Flags API
  slug: featureflip-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-feature-flags-api-openapi.yml
- filename: featureflip-me-api-openapi.yml
  format: yaml
  label: Featureflip Me API
  slug: featureflip-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-me-api-openapi.yml
- filename: featureflip-organizations-api-openapi.yml
  format: yaml
  label: Featureflip Organizations API
  slug: featureflip-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-organizations-api-openapi.yml
- filename: featureflip-projects-api-openapi.yml
  format: yaml
  label: Featureflip Projects API
  slug: featureflip-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-projects-api-openapi.yml
- filename: featureflip-sdk-keys-api-openapi.yml
  format: yaml
  label: Featureflip SDK Keys API
  slug: featureflip-sdk-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-sdk-keys-api-openapi.yml
- filename: featureflip-server-sdk-api-openapi.yml
  format: yaml
  label: Featureflip Server SDK API
  slug: featureflip-server-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-server-sdk-api-openapi.yml
- filename: featureflip-user-segments-api-openapi.yml
  format: yaml
  label: Featureflip User Segments API
  slug: featureflip-user-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/openapi/featureflip-user-segments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: featureflip.io
  spf: true
hosts:
- cert_expires: Dec 10 11:33:13 2026 GMT
  host: featureflip.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 11:38:42 2026 GMT
  host: api.featureflip.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 11:38:42 2026 GMT
  host: eval.featureflip.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Featureflip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Featureflip, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Featureflip
provider_slug: featureflip
slug: featureflip-domain-security
source_filename: featureflip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: featureflip.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 11:33:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.featureflip.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 11:38:42 2026 GMT\n  hsts: null\n- host: eval.featureflip.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 11:38:42 2026 GMT\n  hsts: null\ndomains:\n- domain: featureflip.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/featureflip/refs/heads/main/security/featureflip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Feature Flags
- Feature Management
- feature flag cleanup
- Progressive Delivery
- Experimentation
- feature flags as code
- OpenFeature
- MCP
- Developer Tools
- DevOps/CI-CD
---

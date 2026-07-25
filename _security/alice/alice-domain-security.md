---
api_specs:
- filename: alice-api-keys-api-openapi.yml
  format: yaml
  label: Alice api keys API
  slug: alice-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-api-keys-api-openapi.yml
- filename: alice-collection-api-openapi.yml
  format: yaml
  label: Alice collection API
  slug: alice-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-collection-api-openapi.yml
- filename: alice-content-api-openapi.yml
  format: yaml
  label: Alice content API
  slug: alice-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-content-api-openapi.yml
- filename: alice-flags-api-openapi.yml
  format: yaml
  label: Alice flags API
  slug: alice-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-flags-api-openapi.yml
- filename: alice-users-api-openapi.yml
  format: yaml
  label: Alice users API
  slug: alice-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-users-api-openapi.yml
- filename: alice-wonderbuild-api-openapi.yml
  format: yaml
  label: Alice WonderBuild API
  slug: alice-wonderbuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-wonderbuild-api-openapi.yml
- filename: alice-wonderfence-api-openapi.yml
  format: yaml
  label: Alice WonderFence API
  slug: alice-wonderfence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-wonderfence-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alice.io
  spf: true
hosts:
- cert_expires: Sep 24 08:46:42 2026 GMT
  host: alice.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 12:42:14 2026 GMT
  host: api.alice.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alice, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alice
provider_slug: alice
slug: alice-domain-security
source_filename: alice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alice.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:46:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alice.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:42:14 2026 GMT\n  hsts: null\ndomains:\n- domain: alice.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/security/alice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- AI Security
- AI Safety
- Content Moderation
- Trust and Safety
- LLM Guardrails
- Red Teaming
- GenAI
---

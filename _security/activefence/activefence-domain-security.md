---
api_specs:
- filename: activefence-api-keys-api-openapi.yml
  format: yaml
  label: ActiveFence api keys API
  slug: activefence-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-api-keys-api-openapi.yml
- filename: activefence-collection-api-openapi.yml
  format: yaml
  label: ActiveFence Collection API
  slug: activefence-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-collection-api-openapi.yml
- filename: activefence-content-api-openapi.yml
  format: yaml
  label: ActiveFence Content API
  slug: activefence-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-content-api-openapi.yml
- filename: activefence-flags-api-openapi.yml
  format: yaml
  label: ActiveFence Flags API
  slug: activefence-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-flags-api-openapi.yml
- filename: activefence-users-api-openapi.yml
  format: yaml
  label: ActiveFence Users API
  slug: activefence-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-users-api-openapi.yml
- filename: activefence-wonderbuild-api-openapi.yml
  format: yaml
  label: ActiveFence Wonder Build API
  slug: activefence-wonderbuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-wonderbuild-api-openapi.yml
- filename: activefence-wonderfence-api-openapi.yml
  format: yaml
  label: ActiveFence Wonder Fence API
  slug: activefence-wonderfence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-wonderfence-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alice.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: activefence.com
  spf: true
hosts:
- cert_expires: Sep 24 08:46:42 2026 GMT
  host: alice.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: docs.activefence.com
  hsts: false
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
name: Activefence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ActiveFence, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ActiveFence
provider_slug: activefence
slug: activefence-domain-security
source_filename: activefence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alice.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:46:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.activefence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.alice.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:42:14 2026 GMT\n  hsts: null\ndomains:\n- domain: alice.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: activefence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/security/activefence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Safety
- AI Security
- Trust and Safety
- Content Moderation
- Guardrails
- Red Teaming
- LLM Security
- Prompt Injection
- AI Governance
- Risk Scoring
- User Generated Content
- Child Safety
---

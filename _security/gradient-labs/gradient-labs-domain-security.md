---
api_specs:
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Conversations API
  slug: gradient-labs-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Messages API
  slug: gradient-labs-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Hand-off & Assignment API
  slug: gradient-labs-hand-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Actions & Tools API
  slug: gradient-labs-actions-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Knowledge API
  slug: gradient-labs-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Webhooks API
  slug: gradient-labs-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gradient-labs.ai
  spf: true
hosts:
- cert_expires: Oct  4 05:26:59 2026 GMT
  host: www.gradient-labs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 15:24:06 2026 GMT
  host: api-docs.gradient-labs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 10:16:14 2026 GMT
  host: api.gradient-labs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gradient Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gradient Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gradient Labs
provider_slug: gradient-labs
slug: gradient-labs-domain-security
source_filename: gradient-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gradient-labs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:26:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.gradient-labs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:24:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gradient-labs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:16:14 2026 GMT\n  hsts: null\ndomains:\n- domain: gradient-labs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/security/gradient-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Customer Support
- AI Agent
- Conversations
- Financial Services
- Regulated
---

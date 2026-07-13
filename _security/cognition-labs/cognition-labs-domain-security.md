---
api_specs:
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Sessions API
  slug: devin-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Messages API
  slug: devin-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Attachments API
  slug: devin-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Knowledge API
  slug: devin-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Playbooks API
  slug: devin-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Secrets API
  slug: devin-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Organizations API
  slug: devin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Enterprise API
  slug: devin-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
- filename: cognition-labs-openapi.yml
  format: yaml
  label: Devin Usage & Consumption API
  slug: devin-usage-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/openapi/cognition-labs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognition.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: devin.ai
  spf: true
hosts:
- cert_expires: Sep 15 04:25:43 2026 GMT
  host: cognition.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 22:34:00 2026 GMT
  host: docs.devin.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api.devin.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognition Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognition Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cognition Labs
provider_slug: cognition-labs
slug: cognition-labs-domain-security
source_filename: cognition-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognition.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:25:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.devin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 22:34:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.devin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cognition.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: devin.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognition-labs/refs/heads/main/security/cognition-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- AI Agent
- Autonomous Coding
- Software Engineering
- LLM
- Devin
---

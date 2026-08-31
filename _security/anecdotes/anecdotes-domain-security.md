---
api_specs:
- filename: anecdotes-analysis-rules-api-openapi.yml
  format: yaml
  label: anecdotes Analysis Rules API
  slug: anecdotes-analysis-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-analysis-rules-api-openapi.yml
- filename: anecdotes-authorization-api-openapi.yml
  format: yaml
  label: anecdotes Authorization API
  slug: anecdotes-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-authorization-api-openapi.yml
- filename: anecdotes-create-controls-api-openapi.yml
  format: yaml
  label: anecdotes Create Controls API
  slug: anecdotes-create-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-create-controls-api-openapi.yml
- filename: anecdotes-create-evidence-api-openapi.yml
  format: yaml
  label: anecdotes Create Evidence API
  slug: anecdotes-create-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-create-evidence-api-openapi.yml
- filename: anecdotes-custom-fields-api-openapi.yml
  format: yaml
  label: anecdotes Custom Fields API
  slug: anecdotes-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-custom-fields-api-openapi.yml
- filename: anecdotes-download-evidence-api-openapi.yml
  format: yaml
  label: anecdotes Download Evidence API
  slug: anecdotes-download-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-download-evidence-api-openapi.yml
- filename: anecdotes-findings-api-openapi.yml
  format: yaml
  label: anecdotes Findings API
  slug: anecdotes-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-findings-api-openapi.yml
- filename: anecdotes-framework-api-openapi.yml
  format: yaml
  label: anecdotes Framework API
  slug: anecdotes-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-framework-api-openapi.yml
- filename: anecdotes-gated-api-openapi.yml
  format: yaml
  label: anecdotes Gated API
  slug: anecdotes-gated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-gated-api-openapi.yml
- filename: anecdotes-policy-manager-api-openapi.yml
  format: yaml
  label: anecdotes Policy Manager API
  slug: anecdotes-policy-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-policy-manager-api-openapi.yml
- filename: anecdotes-public-api-openapi.yml
  format: yaml
  label: anecdotes Public API
  slug: anecdotes-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-public-api-openapi.yml
- filename: anecdotes-read-controls-api-openapi.yml
  format: yaml
  label: anecdotes Read Controls API
  slug: anecdotes-read-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-read-controls-api-openapi.yml
- filename: anecdotes-read-evidence-metadata-api-openapi.yml
  format: yaml
  label: anecdotes Read Evidence Metadata API
  slug: anecdotes-read-evidence-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-read-evidence-metadata-api-openapi.yml
- filename: anecdotes-requirements-api-openapi.yml
  format: yaml
  label: anecdotes Requirements API
  slug: anecdotes-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-requirements-api-openapi.yml
- filename: anecdotes-risk-api-openapi.yml
  format: yaml
  label: anecdotes Risk API
  slug: anecdotes-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-risk-api-openapi.yml
- filename: anecdotes-token-api-openapi.yml
  format: yaml
  label: anecdotes Token API
  slug: anecdotes-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-token-api-openapi.yml
- filename: anecdotes-update-control-metadata-api-openapi.yml
  format: yaml
  label: anecdotes Update Control Metadata API
  slug: anecdotes-update-control-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-update-control-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anecdotes.ai
  spf: true
hosts:
- cert_expires: Oct 14 22:48:49 2026 GMT
  host: www.anecdotes.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:32:57 2026 GMT
  host: help.anecdotes.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 17:09:16 2026 GMT
  host: api.anecdotes.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anecdotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anecdotes, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: anecdotes
provider_slug: anecdotes
slug: anecdotes-domain-security
source_filename: anecdotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anecdotes.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:48:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.anecdotes.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anecdotes.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:09:16 2026 GMT\n  hsts: null\ndomains:\n- domain: anecdotes.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/security/anecdotes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Compliance
- Governance
- Risk
- Security
- GRC
- Audit
- Evidence
- Continuous Compliance
- FedRAMP
- Artificial Intelligence
- Agents
---

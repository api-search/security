---
api_specs:
- filename: autoderm-ai-dermatology-api-device-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Device API
  slug: autoderm-ai-dermatology-api-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-device-api-openapi.yml
- filename: autoderm-ai-dermatology-api-inference-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Inference API
  slug: autoderm-ai-dermatology-api-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-inference-api-openapi.yml
- filename: autoderm-ai-dermatology-api-system-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API System API
  slug: autoderm-ai-dermatology-api-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-system-api-openapi.yml
- filename: autoderm-ai-dermatology-api-utils-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Utils API
  slug: autoderm-ai-dermatology-api-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-utils-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autoderm.ai
  spf: true
hosts:
- cert_expires: Oct 14 16:55:14 2026 GMT
  host: docs.autoderm.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 01:43:21 2026 GMT
  host: autoderm.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 01:43:21 2026 GMT
  host: api.autoderm.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autoderm Ai Dermatology Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autoderm – AI Dermatology API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Autoderm – AI Dermatology API
provider_slug: autoderm-ai-dermatology-api
slug: autoderm-ai-dermatology-api-domain-security
source_filename: autoderm-ai-dermatology-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.autoderm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:55:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: autoderm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 01:43:21 2026 GMT\n  hsts: false\n- host: api.autoderm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 01:43:21 2026 GMT\n  hsts: null\ndomains:\n- domain: autoderm.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/security/autoderm-ai-dermatology-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- dermatology-api
- ai-dermatology
- medical-imaging
- telemedicine
- skin-analysis
- rest-api
- openapi
- llms-txt
- ce-marked
- white-label
- healthcare
- medical-ai
- computer-vision
- medical-device
- icd-10
- image-classification
- clinical-decision-support
- triage
---

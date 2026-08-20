---
api_specs:
- filename: pixee-ai-findings-api-openapi.yml
  format: yaml
  label: Pixee Findings API
  slug: pixee-ai-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-findings-api-openapi.yml
- filename: pixee-ai-fixes-api-openapi.yml
  format: yaml
  label: Pixee Fixes API
  slug: pixee-ai-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-fixes-api-openapi.yml
- filename: pixee-ai-repositories-api-openapi.yml
  format: yaml
  label: Pixee Repositories API
  slug: pixee-ai-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-repositories-api-openapi.yml
- filename: pixee-ai-scans-api-openapi.yml
  format: yaml
  label: Pixee Scans API
  slug: pixee-ai-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-scans-api-openapi.yml
- filename: pixee-ai-webhooks-api-openapi.yml
  format: yaml
  label: Pixee Webhooks API
  slug: pixee-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pixee.ai
  spf: true
hosts:
- cert_expires: Oct  1 10:31:16 2026 GMT
  host: www.pixee.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixee Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pixee
provider_slug: pixee-ai
slug: pixee-ai-domain-security
source_filename: pixee-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pixee.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pixee.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/security/pixee-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Application Security
- AppSec
- Vulnerability Remediation
- Static Analysis
- SARIF
- Code Security
- Artificial Intelligence
- Developer Tools
---

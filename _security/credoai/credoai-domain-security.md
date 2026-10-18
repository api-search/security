---
api_specs:
- filename: credoai-audit-logs-api-openapi.yml
  format: yaml
  label: Credoai Audit Logs API
  slug: credoai-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/openapi/credoai-audit-logs-api-openapi.yml
- filename: credoai-shadow-ai-api-openapi.yml
  format: yaml
  label: Credoai Shadow AI API
  slug: credoai-shadow-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/openapi/credoai-shadow-ai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: credo.ai
  spf: true
hosts:
- cert_expires: Dec 24 02:27:41 2026 GMT
  host: www.credo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credoai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credoai
provider_slug: credoai
slug: credoai-domain-security
source_filename: credoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 02:27:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: credo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/security/credoai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Governance
- Software-as-a-Service
- PaloAlto
---

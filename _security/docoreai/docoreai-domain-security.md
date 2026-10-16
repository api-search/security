---
api_specs:
- filename: docoreai-openapi-generated.yml
  format: yaml
  label: DoCoreAI API
  slug: docoreai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docoreai/refs/heads/main/openapi/_ae-authored/docoreai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docoreai.com
  spf: true
hosts:
- cert_expires: Nov 27 15:54:49 2026 GMT
  host: docoreai.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docoreai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoCoreAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DoCoreAI
provider_slug: docoreai
slug: docoreai-domain-security
source_filename: docoreai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docoreai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 15:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: docoreai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docoreai/refs/heads/main/security/docoreai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Governance
- Cost Management
- LLM
- SaaS
---

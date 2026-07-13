---
api_specs:
- filename: protectai-openapi.yml
  format: yaml
  label: LLM Guard (Scanners)
  slug: llm-guard-scanners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protectai/refs/heads/main/openapi/protectai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: protectai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: llm-guard.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: protectai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: llm-guard.com
  https: false
kind: domain-security
layout: security
method: probed
name: Protectai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protect AI, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Protect AI
provider_slug: protectai
slug: protectai-domain-security
source_filename: protectai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: protectai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: llm-guard.com\n  https: false\ndomains:\n- domain: protectai.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: llm-guard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protectai/refs/heads/main/security/protectai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- ML
- Security
- LLM
- Guardrails
---

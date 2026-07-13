---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: guardrailsai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nvidia.com
  spf: true
hosts:
- cert_expires: Sep 14 09:48:44 2026 GMT
  host: www.guardrailsai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.guardrailsai.com
  https: false
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: docs.nvidia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guardrails Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Guardrails, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AI Guardrails
provider_slug: guardrails
slug: guardrails-domain-security
source_filename: guardrails-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guardrailsai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:48:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.guardrailsai.com\n  https: false\n- host: docs.nvidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: guardrailsai.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nvidia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardrails/refs/heads/main/security/guardrails-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Safety
- AI Security
- Content Moderation
- Guardrails
- Jailbreak Detection
- LLM Security
- PII Detection
- Prompt Injection
- Responsible AI
---

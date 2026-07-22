---
api_specs:
- filename: eng-api
  format: yaml
  label: TrojAI Platform API
  slug: trojai-platform-api
  spec_type: OpenAPI
  url: https://docs.troj.ai/reference/eng-api
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@troj.ai"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: troj.ai
  spf: true
hosts:
- cert_expires: Sep 30 20:36:13 2026 GMT
  host: troj.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trojai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrojAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TrojAI
provider_slug: trojai
slug: trojai-domain-security
source_filename: trojai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: troj.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:36:13 2026 GMT\n  hsts: false\ndomains:\n- domain: troj.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@troj.ai\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trojai/refs/heads/main/security/trojai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- AI Security
- Machine Learning
- LLM Security
- Red Teaming
- AI Firewall
- Prompt Injection
- Model Risk
- MLOps
- Agentic AI
---

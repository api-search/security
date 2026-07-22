---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paxton.ai
  spf: true
hosts:
- cert_expires: Oct  1 20:13:42 2026 GMT
  host: www.paxton.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paxton Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paxton AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paxton AI
provider_slug: paxton-ai
slug: paxton-ai-domain-security
source_filename: paxton-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paxton.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paxton.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paxton-ai/refs/heads/main/security/paxton-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Legal AI
- LegalTech
- Legal Research
- Legal Drafting
- Document Analysis
- Case Law
- Regulations
- Medical Chronologies
- Discovery
- Depositions
- Generative AI
- Vertical AI
- Law Firms
- Attorneys
- SaaS
---

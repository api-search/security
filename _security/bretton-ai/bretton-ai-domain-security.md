---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bretton.com
  spf: true
hosts:
- cert_expires: Aug 24 04:32:30 2026 GMT
  host: www.bretton.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bretton Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bretton AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bretton AI
provider_slug: bretton-ai
slug: bretton-ai-domain-security
source_filename: bretton-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bretton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:32:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bretton.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bretton-ai/refs/heads/main/security/bretton-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- RegTech
- Financial Crime
- Compliance
- AML
- KYC
- AI Agents
- Artificial Intelligence
---

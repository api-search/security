---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lotus.ai
  spf: true
hosts:
- cert_expires: Oct 13 14:30:25 2026 GMT
  host: lotus.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lotus Health Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lotus Health AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lotus Health AI
provider_slug: lotus-health-ai
slug: lotus-health-ai-domain-security
source_filename: lotus-health-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lotus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 14:30:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lotus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lotus-health-ai/refs/heads/main/security/lotus-health-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Telehealth
- Digital Health
- Consumer
- Medical Records
- Prescriptions
---

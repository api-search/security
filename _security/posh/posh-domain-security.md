---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: posh.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: poshdevelopment.com
  spf: true
hosts:
- cert_expires: Oct 16 10:03:15 2026 GMT
  host: www.posh.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:42:56 2026 GMT
  host: api.poshdevelopment.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Posh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Posh, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Posh
provider_slug: posh
slug: posh-domain-security
source_filename: posh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.posh.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:03:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.poshdevelopment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:42:56 2026 GMT\n  hsts: null\ndomains:\n- domain: posh.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: poshdevelopment.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posh/refs/heads/main/security/posh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Conversational AI
- Agentic AI
- Banking
- Credit Unions
- Financial-Services
- Customer Service
- Contact Center
- Voice
- Chatbots
- Knowledge-Management
- RegTech
---

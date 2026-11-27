---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: sumgenius.ai
  spf: true
hosts:
- cert_expires: Jan 22 12:20:57 2027 GMT
  host: sumgenius.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SumGeniusAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SumGeniusAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SumGeniusAI
provider_slug: sumgenius-ai
slug: sumgenius-ai-domain-security
source_filename: sumgenius-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sumgenius.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 12:20:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sumgenius.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sumgenius-ai/security/sumgenius-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chatbot
- DM Automation
- Appointment Booking
- Lead Capture
- Content Scheduling
---

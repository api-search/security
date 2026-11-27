---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nevent.ai
  spf: false
hosts:
- cert_expires: May 24 12:00:14 2027 GMT
  host: nevent.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nevent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nevent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Nevent
provider_slug: nevent-ai
slug: nevent-ai-domain-security
source_filename: nevent-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nevent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 24 12:00:14 2027 GMT\n  hsts: false\ndomains:\n- domain: nevent.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nevent-ai/security/nevent-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Event Marketing
- CRM
- Email Marketing
- SMS
- AI Chatbot
- Audience Insights
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aiug.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: travl.app
  spf: true
hosts:
- cert_expires: Mar  3 17:25:06 2027 GMT
  host: www.aiug.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 00:02:37 2026 GMT
  host: www.travl.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.lever.app
  http_status: 503
  https: true
  note: 'Render service suspended (x-render-routing: suspend); host resolves and terminates TLS but serves no application.'
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ai Unlimited Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Unlimited Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AI Unlimited Group
provider_slug: ai-unlimited-group
slug: ai-unlimited-group-domain-security
source_filename: ai-unlimited-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aiug.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 17:25:06 2027 GMT\n  hsts: false\n- host: www.travl.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 00:02:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lever.app\n  https: true\n  tls_version: TLSv1.3\n  http_status: 503\n  note: 'Render service suspended (x-render-routing: suspend); host resolves and terminates\n    TLS but serves no application.'\ndomains:\n- domain: aiug.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: travl.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nx-note: >-\n  www.aiug.ai is a GoDaddy parking lander, not a running application; the TLS/DNS posture\n  recorded for it is the parking host's, not the company's. travl.app is the only live\n  company-operated web property probed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-unlimited-group/refs/heads/main/security/ai-unlimited-group-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Fintech
- Consumer Finance
- Debt Management
- Travel
- Investing
- Mobile App
---

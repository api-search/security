---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognigy.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognigy.ai
  spf: true
hosts:
- cert_expires: Sep 13 21:19:31 2026 GMT
  host: www.cognigy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 07:13:07 2026 GMT
  host: docs.cognigy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 12:22:15 2026 GMT
  host: api-app.cognigy.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognigy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognigy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cognigy
provider_slug: cognigy
slug: cognigy-domain-security
source_filename: cognigy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognigy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:19:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cognigy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-app.cognigy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 12:22:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cognigy.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cognigy.ai\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognigy/refs/heads/main/security/cognigy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Conversational AI
- Agentic AI
- Contact Center
- Customer Service Automation
- Chatbots
- Voice AI
- Virtual Agents
- Enterprise AI
- Omnichannel
---

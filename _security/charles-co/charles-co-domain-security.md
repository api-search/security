---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hello-charles.com
  spf: true
hosts:
- cert_expires: Sep 30 19:23:00 2026 GMT
  host: www.hello-charles.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 03:42:47 2026 GMT
  host: api.hello-charles.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charles Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charles Co, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Charles Co
provider_slug: charles-co
slug: charles-co-domain-security
source_filename: charles-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hello-charles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:23:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hello-charles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: hello-charles.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charles-co/refs/heads/main/security/charles-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Conversational Commerce
- Messaging
- WhatsApp
- CRM
- Customer Support
- E-Commerce
- AI Agents
---

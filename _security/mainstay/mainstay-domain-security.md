---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mainstay.com
  spf: true
hosts:
- cert_expires: Oct 11 05:15:02 2026 GMT
  host: www.mainstay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mainstay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mainstay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mainstay
provider_slug: mainstay
slug: mainstay-domain-security
source_filename: mainstay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mainstay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:15:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mainstay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mainstay/refs/heads/main/security/mainstay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Higher Education
- Conversational AI
- Student Engagement
- Chatbot
- Messaging
---

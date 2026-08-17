---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atomchat.io
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudfunctions.net
  spf: true
hosts:
- cert_expires: Oct 28 12:13:03 2026 GMT
  host: atomchat.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 03:55:52 2026 GMT
  host: soporte.atomchat.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:06:28 2026 GMT
  host: us-central1-atomchat-io.cloudfunctions.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATOM, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ATOM
provider_slug: atom
slug: atom-domain-security
source_filename: atom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomchat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 12:13:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: soporte.atomchat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:55:52 2026 GMT\n  hsts: null\n- host: us-central1-atomchat-io.cloudfunctions.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:06:28 2026 GMT\n  hsts: null\ndomains:\n- domain: atomchat.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cloudfunctions.net\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atom/refs/heads/main/security/atom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Messaging
- WhatsApp
- Artificial Intelligence
- Conversational Commerce
- Chatbots
- Sales
- Lead Generation
- Customer Engagement
- Latin America
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: burnerapp.com
  spf: true
hosts:
- cert_expires: Aug 26 07:14:51 2026 GMT
  host: burnerapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Burner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Burner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Burner
provider_slug: burner
slug: burner-domain-security
source_filename: burner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: burnerapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:14:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: burnerapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burner/refs/heads/main/security/burner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Phone Numbers
- SMS
- MMS
- Voice
- Messaging
- Telephony
- Privacy
- Communications
- Second Phone Number
- OAuth
- Webhooks
---

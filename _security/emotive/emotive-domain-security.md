---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emotive.io
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: emotive.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emotive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emotive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Emotive
provider_slug: emotive
slug: emotive-domain-security
source_filename: emotive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emotive.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: emotive.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/security/emotive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- SMS
- Messaging
- eCommerce
- Marketing Automation
- Text Message Marketing
- Conversational Commerce
---

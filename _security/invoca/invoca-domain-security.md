---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: invoca.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: invoca.net
  spf: true
hosts:
- cert_expires: Oct 15 10:48:48 2026 GMT
  host: www.invoca.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 09:08:26 2026 GMT
  host: developers.invoca.net
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: invoca.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Invoca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invoca, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Invoca
provider_slug: invoca
slug: invoca-domain-security
source_filename: invoca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.invoca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:48:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.invoca.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:08:26 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: invoca.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: invoca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: invoca.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invoca/refs/heads/main/security/invoca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Call Tracking
- Conversation Intelligence
- Marketing
- Attribution
- Revenue
- Telephony
- Analytics
---

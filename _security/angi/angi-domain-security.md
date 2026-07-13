---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: angi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intercom.help
  spf: false
hosts:
- cert_expires: Oct  6 19:46:14 2026 GMT
  host: www.angi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: intercom.help
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 00:40:11 2026 GMT
  host: help.servicetitan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Angi
provider_slug: angi
slug: angi-domain-security
source_filename: angi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.angi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:46:14 2026 GMT\n  hsts: false\n- host: intercom.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.servicetitan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 00:40:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: angi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: intercom.help\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angi/refs/heads/main/security/angi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Services
- Marketplace
- Leads
- Angie's List
- HomeAdvisor
- IAC
- Webhook
- No Public API
---

---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: embroker.com
  spf: true
hosts:
- cert_expires: Aug 22 01:38:35 2026 GMT
  host: www.embroker.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Embroker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Embroker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Embroker
provider_slug: embroker
slug: embroker-domain-security
source_filename: embroker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.embroker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 01:38:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: embroker.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embroker/refs/heads/main/security/embroker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Business Insurance
- Commercial Insurance
- Insurtech
- Digital Insurance
- Broker
- Managing General Agent
- Cyber Insurance
- Professional Liability
- Directors and Officers
- Startups
- Law Firms
- Risk Management
---

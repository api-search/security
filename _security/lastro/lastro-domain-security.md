---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lastro.co
  spf: true
hosts:
- cert_expires: Aug 29 17:08:35 2026 GMT
  host: lastro.co
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lastro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lastro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lastro
provider_slug: lastro
slug: lastro-domain-security
source_filename: lastro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lastro.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:08:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: lastro.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastro/refs/heads/main/security/lastro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Real Estate
- Artificial Intelligence
- Brazil
- Lead Management
- Conversational AI
- WhatsApp
---

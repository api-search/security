---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: floatbot.ai
  spf: true
hosts:
- cert_expires: Jan 29 06:03:47 2027 GMT
  host: floatbot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Floatbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Floatbot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Floatbot
provider_slug: floatbot
slug: floatbot-domain-security
source_filename: floatbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: floatbot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 06:03:47 2027 GMT\n  hsts: null\ndomains:\n- domain: floatbot.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/floatbot/security/floatbot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Platform
- Conversational AI
- Voice AI
- Insurance
- Collection
- Healthcare
- Banking
- Lending
---

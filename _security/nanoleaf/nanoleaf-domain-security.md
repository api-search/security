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
  domain: nanoleaf.me
  spf: true
hosts:
- cert_expires: Jan  8 10:58:02 2027 GMT
  host: nanoleaf.me
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nanoleaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanoleaf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nanoleaf
provider_slug: nanoleaf
slug: nanoleaf-domain-security
source_filename: nanoleaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nanoleaf.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 10:58:02 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: nanoleaf.me\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nanoleaf/security/nanoleaf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Lighting
- IoT
- Home Automation
- AI
---

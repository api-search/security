---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prizepicks.com
  spf: true
hosts:
- cert_expires: Oct  7 00:58:07 2026 GMT
  host: prizepicks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prizepicks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrizePicks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PrizePicks
provider_slug: prizepicks
slug: prizepicks-domain-security
source_filename: prizepicks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prizepicks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:58:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prizepicks.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prizepicks/refs/heads/main/security/prizepicks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Daily Fantasy Sports
- Player Props
- Pick-em
- Gaming
- Regulated
---

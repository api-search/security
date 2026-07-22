---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "identrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caseys.com
  spf: true
hosts:
- cert_expires: Dec 11 17:06:35 2026 GMT
  host: www.caseys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caseys General Stores Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casey''s General Stores, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Casey's General Stores
provider_slug: caseys-general-stores
slug: caseys-general-stores-domain-security
source_filename: caseys-general-stores-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caseys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 17:06:35 2026 GMT\n  hsts: null\ndomains:\n- domain: caseys.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caseys-general-stores/refs/heads/main/security/caseys-general-stores-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Convenience Stores
- Food Service
- Fortune 500
- Fuel Retail
- Loyalty
- Pizza
- Retail
---

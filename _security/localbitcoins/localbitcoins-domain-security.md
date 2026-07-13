---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa@localbitcoins.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: localbitcoins.com
  spf: false
hosts:
- cert_expires: Sep  4 19:30:50 2026 GMT
  host: localbitcoins.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Localbitcoins Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Localbitcoins, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Localbitcoins
provider_slug: localbitcoins
slug: localbitcoins-domain-security
source_filename: localbitcoins-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localbitcoins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: localbitcoins.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa@localbitcoins.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localbitcoins/refs/heads/main/security/localbitcoins-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Public APIs
---

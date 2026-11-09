---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: destaire.com
  spf: true
hosts:
- cert_expires: Feb  2 15:18:40 2027 GMT
  host: destaire.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Destaire Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Destaire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Destaire
provider_slug: destaire-com
slug: destaire-com-domain-security
source_filename: destaire-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: destaire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 15:18:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: destaire.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/destaire-com/security/destaire-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Hospitality
- Curated Guides
- Luxury
- Destination
---

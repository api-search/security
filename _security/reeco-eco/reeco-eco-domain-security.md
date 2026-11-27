---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:admin@stefanociprianistudio.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-23'
    published: false
  dnssec: true
  domain: reeco.eco
  spf: true
hosts:
- cert_expires: Feb 17 12:15:32 2027 GMT
  host: reeco.eco
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reeco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reeco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Reeco
provider_slug: reeco-eco
slug: reeco-eco-domain-security
source_filename: reeco-eco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reeco.eco\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 12:15:32 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: reeco.eco\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:admin@stefanociprianistudio.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-23'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reeco-eco/security/reeco-eco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Textile
- Sustainability
- DigitalProductPassport
- Verification
- AI
---

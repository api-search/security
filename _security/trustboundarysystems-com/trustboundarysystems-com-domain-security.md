---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@trustboundarysystems.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: trustboundarysystems.com
  spf: true
hosts:
- cert_expires: Jan 11 00:18:49 2027 GMT
  host: trustboundarysystems.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trust Boundary Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trust Boundary Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trust Boundary Systems
provider_slug: trustboundarysystems-com
slug: trustboundarysystems-com-domain-security
source_filename: trustboundarysystems-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustboundarysystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 00:18:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trustboundarysystems.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@trustboundarysystems.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/trustboundarysystems-com/security/trustboundarysystems-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- AI
- Security
- Financial Services
- Consulting
---

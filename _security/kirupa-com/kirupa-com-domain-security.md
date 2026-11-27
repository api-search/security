---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: kirupa.com
  spf: true
hosts:
- cert_expires: Jan 16 08:23:22 2027 GMT
  host: kirupa.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kirupa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kirupa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Kirupa
provider_slug: kirupa-com
slug: kirupa-com-domain-security
source_filename: kirupa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kirupa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 08:23:22 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: kirupa.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kirupa-com/security/kirupa-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Education
- Tutorials
- Web Development
- Design
- Community
---

---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: false
  domain: auriniaxo.com
  spf: false
hosts:
- cert_expires: Jan 29 16:00:09 2027 GMT
  host: auriniaxo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auriniaxo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AURINIA XO HOSTEL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AURINIA XO HOSTEL
provider_slug: auriniaxo-com
slug: auriniaxo-com-domain-security
source_filename: auriniaxo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auriniaxo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 16:00:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: auriniaxo.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/auriniaxo-com/security/auriniaxo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Hostel
- Accommodation
- Ukraine
- Budget Travel
- Kamianets-Podilskyi
---

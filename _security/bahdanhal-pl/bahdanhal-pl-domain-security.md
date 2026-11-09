---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "certum.pl"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: bahdanhal.pl
  spf: true
hosts:
- cert_expires: Dec  3 18:26:15 2026 GMT
  host: bahdanhal.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bahdanhal Pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bahdan Hal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bahdan Hal
provider_slug: bahdanhal-pl
slug: bahdanhal-pl-domain-security
source_filename: bahdanhal-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bahdanhal.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 18:26:15 2026 GMT\n  hsts: false\ndomains:\n- domain: bahdanhal.pl\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"certum.pl\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bahdanhal-pl/security/bahdanhal-pl-domain-security.yml
summary_line: TLSv1.3
tags:
- Backend
- Engineer
- Symfony
- Laravel
- Artificial Intelligence
- Poland
---

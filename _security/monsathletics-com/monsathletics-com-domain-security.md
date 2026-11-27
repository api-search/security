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
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monsathletics.com
  spf: true
hosts:
- cert_expires: Dec 28 11:09:38 2026 GMT
  host: monsathletics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MONS Athletics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MONS Athletics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MONS Athletics
provider_slug: monsathletics-com
slug: monsathletics-com-domain-security
source_filename: monsathletics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monsathletics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 11:09:38 2026 GMT\n  hsts: false\ndomains:\n- domain: monsathletics.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/monsathletics-com/security/monsathletics-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports
- Coaching
- Fitness
- Triathlon
- Apple
---

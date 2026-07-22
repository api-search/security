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
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: speedhome.com
  spf: true
hosts:
- cert_expires: Sep  1 15:10:48 2026 GMT
  host: speedhome.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speedhome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpeedHome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpeedHome
provider_slug: speedhome
slug: speedhome-domain-security
source_filename: speedhome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: speedhome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:10:48 2026 GMT\n  hsts: null\ndomains:\n- domain: speedhome.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speedhome/refs/heads/main/security/speedhome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Property Rental
- Marketplace
- Proptech
- Malaysia
- Consumer
---

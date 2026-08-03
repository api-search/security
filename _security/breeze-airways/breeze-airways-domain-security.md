---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flybreeze.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: navitaire.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.flybreeze.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 04:40:58 2026 GMT
  host: ndc.flybreeze.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: ndcr4y.prod.mx.navitaire.com
  https: false
kind: domain-security
layout: security
method: probed
name: Breeze Airways Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breeze Airways, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Breeze Airways
provider_slug: breeze-airways
slug: breeze-airways-domain-security
source_filename: breeze-airways-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flybreeze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n- host: ndc.flybreeze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 04:40:58 2026 GMT\n  hsts: false\n- host: ndcr4y.prod.mx.navitaire.com\n  https: false\ndomains:\n- domain: flybreeze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: navitaire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze-airways/refs/heads/main/security/breeze-airways-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Airlines
- Travel
- Aviation
- NDC
- Distribution
- Booking
- Reservations
- Travel Agencies
- IATA
---

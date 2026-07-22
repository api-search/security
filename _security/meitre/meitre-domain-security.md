---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meitre.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meitre-api.com
  spf: false
hosts:
- cert_expires: Sep 25 06:00:24 2026 GMT
  host: meitre.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 18:41:36 2026 GMT
  host: meitre-api.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meitre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meitre, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Meitre
provider_slug: meitre
slug: meitre-domain-security
source_filename: meitre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meitre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:00:24 2026 GMT\n  hsts: false\n- host: meitre-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:41:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meitre.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: meitre-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meitre/refs/heads/main/security/meitre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurants
- Reservations
- Hospitality
- Booking
- Guest Management
- Revenue Management
- Food and Beverage
- Latin America
---

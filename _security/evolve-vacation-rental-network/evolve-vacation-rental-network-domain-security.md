---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: evolve.com
  spf: true
hosts:
- cert_expires: Oct 26 12:15:48 2026 GMT
  host: evolve.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evolve Vacation Rental Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evolve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Evolve
provider_slug: evolve-vacation-rental-network
slug: evolve-vacation-rental-network-domain-security
source_filename: evolve-vacation-rental-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evolve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 12:15:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evolve.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolve-vacation-rental-network/refs/heads/main/security/evolve-vacation-rental-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Travel
- Hospitality
- Vacation Rentals
- Short-Term Rentals
- Property Management
- Real-Estate
- Booking
---

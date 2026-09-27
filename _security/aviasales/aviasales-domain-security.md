---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aviasales.ru
  spf: true
hosts:
- cert_expires: Nov 19 11:09:49 2026 GMT
  host: www.aviasales.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aviasales Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aviasales, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aviasales
provider_slug: aviasales
slug: aviasales-domain-security
source_filename: aviasales-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aviasales.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 11:09:49 2026 GMT\n  hsts: false\ndomains:\n- domain: aviasales.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviasales/refs/heads/main/security/aviasales-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Flights
- Booking
- Russia
---

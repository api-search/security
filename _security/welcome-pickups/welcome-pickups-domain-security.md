---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: welcomepickups.com
  spf: true
hosts:
- cert_expires: Feb  7 10:01:50 2027 GMT
  host: welcomepickups.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Welcome PickUps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Welcome PickUps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Welcome PickUps
provider_slug: welcome-pickups
slug: welcome-pickups-domain-security
source_filename: welcome-pickups-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: welcomepickups.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 10:01:50 2027 GMT\n  hsts: false\ndomains:\n- domain: welcomepickups.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/welcome-pickups/security/welcome-pickups-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Booking
- Transfers
- Tours
---

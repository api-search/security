---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pebblelife.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: pebblelife.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pebble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pebble, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pebble
provider_slug: pebble
slug: pebble-domain-security
source_filename: pebble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pebblelife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: pebblelife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pebble/refs/heads/main/security/pebble-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Electric Vehicles
- Recreational Vehicles
- Consumer Hardware
- Mobility
- Travel
- IoT
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: viarail.ca
  spf: true
hosts:
- cert_expires: Aug 17 04:00:00 2026 GMT
  host: www.viarail.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Via Rail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VIA Rail Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VIA Rail Canada
provider_slug: via-rail
slug: via-rail-domain-security
source_filename: via-rail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.viarail.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 17 04:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: viarail.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/via-rail/refs/heads/main/security/via-rail-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Travel
- Canada
- Rail
- Passenger Rail
- Transit
- GTFS
- Open Data
- Booking
- Distribution
- Travel Agents
- Crown Corporation
- Loyalty
---

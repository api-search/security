---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eptura.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spaceiq.com
  spf: true
hosts:
- cert_expires: Sep 13 09:57:27 2026 GMT
  host: eptura.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 11:15:04 2026 GMT
  host: developer.spaceiq.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 11:15:04 2026 GMT
  host: api.spaceiq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spaceiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpaceIQ, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SpaceIQ
provider_slug: spaceiq
slug: spaceiq-domain-security
source_filename: spaceiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eptura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 09:57:27 2026 GMT\n  hsts: false\n- host: developer.spaceiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 11:15:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.spaceiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 11:15:04 2026 GMT\n  hsts: null\ndomains:\n- domain: eptura.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: spaceiq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceiq/refs/heads/main/security/spaceiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Workplace Management
- Space Management
- Facilities Management
- Desk Booking
- Hoteling
- Meeting Rooms
- Occupancy Analytics
- Real Estate
- Floorplans
- GraphQL
- IWMS
- Eptura
---

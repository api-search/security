---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spacebase.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.spacebase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spacebase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spacebase
provider_slug: spacebase
slug: spacebase-domain-security
source_filename: spacebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spacebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: spacebase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacebase/refs/heads/main/security/spacebase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Meeting Rooms
- Event Spaces
- Coworking
- Workspace Booking
- Venue Marketplace
- Bookings
---

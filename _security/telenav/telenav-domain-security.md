---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: telenav.com
  spf: true
hosts:
- host: telenav.com
  https: false
  notes: Apex host fails the TLS handshake; the site is served from www.telenav.com.
- host: www.telenav.com
  hsts: true
  hsts_max_age: 31536000
  https: true
- host: docs.telenav.com
  hsts: false
  https: true
kind: domain-security
layout: security
method: probed
name: Telenav Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telenav, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Telenav
provider_slug: telenav
slug: telenav-domain-security
source_filename: telenav-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telenav.com\n  https: false\n  notes: Apex host fails the TLS handshake; the site is served from www.telenav.com.\n- host: www.telenav.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.telenav.com\n  https: true\n  hsts: false\ndomains:\n- domain: telenav.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telenav/refs/heads/main/security/telenav-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Mapping
- Navigation
- Location
- Search
- Automotive
- Connected Cars
- EV Charging
- Points of Interest
---

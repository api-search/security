---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: attractiontickets.com
  spf: true
hosts:
- cert_expires: Dec 27 23:12:53 2026 GMT
  host: attractiontickets.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Attraction Tickets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attraction Tickets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Attraction Tickets
provider_slug: attractiontickets-com
slug: attractiontickets-com-domain-security
source_filename: attractiontickets-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attractiontickets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:12:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: attractiontickets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/attractiontickets-com/security/attractiontickets-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ticketing
- Travel
- Orlando
- Disney
- Universal
---

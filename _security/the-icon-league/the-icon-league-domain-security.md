---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theiconleague.com
  spf: true
hosts:
- cert_expires: Sep 30 09:18:03 2026 GMT
  host: www.theiconleague.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Icon League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Icon League, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Icon League
provider_slug: the-icon-league
slug: the-icon-league-domain-security
source_filename: the-icon-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theiconleague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:18:03 2026 GMT\n  hsts: false\ndomains:\n- domain: theiconleague.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-icon-league/refs/heads/main/security/the-icon-league-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Sports
- Football
- Soccer
- Entertainment
- Media
- Livestreaming
- League
---

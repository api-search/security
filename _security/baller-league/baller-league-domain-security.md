---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ballerleague.de
  spf: true
hosts:
- cert_expires: Sep 27 14:32:05 2026 GMT
  host: ballerleague.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baller League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baller League, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Baller League
provider_slug: baller-league
slug: baller-league-domain-security
source_filename: baller-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ballerleague.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:32:05 2026 GMT\n  hsts: false\ndomains:\n- domain: ballerleague.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baller-league/refs/heads/main/security/baller-league-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sport
- Football
- Soccer
- Media
- Entertainment
- Live Streaming
- League
---

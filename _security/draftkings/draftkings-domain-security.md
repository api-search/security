---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: draftkings.com
  spf: true
hosts:
- cert_expires: Aug 26 16:24:58 2026 GMT
  host: www.draftkings.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Draftkings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DraftKings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DraftKings
provider_slug: draftkings
slug: draftkings-domain-security
source_filename: draftkings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.draftkings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 16:24:58 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: draftkings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/draftkings/refs/heads/main/security/draftkings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Daily Fantasy Sports
- Gaming
- iGaming
- Online Casino
- Sports Betting
- Sportsbook
---

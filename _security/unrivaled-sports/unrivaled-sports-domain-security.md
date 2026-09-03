---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unrivaledsports.com
  spf: true
hosts:
- cert_expires: Oct 29 09:22:18 2026 GMT
  host: unrivaledsports.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unrivaled Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unrivaled Sports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unrivaled Sports
provider_slug: unrivaled-sports
slug: unrivaled-sports-domain-security
source_filename: unrivaled-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unrivaledsports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 09:22:18 2026 GMT\n  hsts: false\ndomains:\n- domain: unrivaledsports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unrivaled-sports/refs/heads/main/security/unrivaled-sports-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sports
- Youth Sports
- Baseball
- Softball
- Flag Football
- Events
- Tournaments
- Venues
- Camps
- Recreation
- Private Equity Backed
---

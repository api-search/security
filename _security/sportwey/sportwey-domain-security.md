---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sportwey.com
  spf: false
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: sportwey.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sportwey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sportwey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Sportwey
provider_slug: sportwey
slug: sportwey-domain-security
source_filename: sportwey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportwey.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sportwey.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportwey/refs/heads/main/security/sportwey-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Sports
- Tournaments
- Leagues
- Sports Management
- SaaS
- Facilities
- Academies
- Payments
- Mexico
---

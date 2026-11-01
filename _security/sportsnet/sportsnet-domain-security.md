---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sportsnet.ca
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: sportsnet.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sportsnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sportsnet stats ticker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sportsnet stats ticker
provider_slug: sportsnet
slug: sportsnet-domain-security
source_filename: sportsnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportsnet.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sportsnet.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sportsnet/security/sportsnet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- News
- Canada
- Media
- API
---

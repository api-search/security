---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oddiwire.com
  spf: true
hosts:
- cert_expires: Jan 27 14:37:53 2027 GMT
  host: oddiwire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oddiwire Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for oddiwire-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: oddiwire-com
provider_slug: oddiwire-com
slug: oddiwire-com-domain-security
source_filename: oddiwire-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oddiwire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 14:37:53 2027 GMT\n  hsts: false\ndomains:\n- domain: oddiwire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/oddiwire-com/security/oddiwire-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Esports
- Odds
- Real-time
- Betting
---

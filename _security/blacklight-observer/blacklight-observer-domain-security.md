---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: blacklight.observer
  spf: false
hosts:
- cert_expires: Jan  9 06:56:44 2027 GMT
  host: blacklight.observer
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blacklight Observer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blacklight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Blacklight
provider_slug: blacklight-observer
slug: blacklight-observer-domain-security
source_filename: blacklight-observer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blacklight.observer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 06:56:44 2027 GMT\n  hsts: false\ndomains:\n- domain: blacklight.observer\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/blacklight-observer/security/blacklight-observer-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Finance
- Cryptocurrency
- Analytics
- Market Data
- Polymarket
---

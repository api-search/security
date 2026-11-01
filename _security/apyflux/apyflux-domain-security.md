---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apyflux.com
  spf: true
hosts:
- cert_expires: Apr 13 11:33:08 2027 GMT
  host: apyflux.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apyflux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apyflux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apyflux
provider_slug: apyflux
slug: apyflux-domain-security
source_filename: apyflux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apyflux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 13 11:33:08 2027 GMT\n  hsts: null\ndomains:\n- domain: apyflux.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/apyflux/security/apyflux-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Marketplace
- Developer Tools
- Integration
- Monetization
- Software-as-a-Service
---

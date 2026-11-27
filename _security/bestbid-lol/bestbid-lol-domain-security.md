---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bestbid.lol
  spf: false
hosts:
- cert_expires: Jan 23 03:58:05 2027 GMT
  host: bestbid.lol
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BestBid.lol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BestBid.lol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: BestBid.lol
provider_slug: bestbid-lol
slug: bestbid-lol-domain-security
source_filename: bestbid-lol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bestbid.lol\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 03:58:05 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bestbid.lol\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bestbid-lol/security/bestbid-lol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Marketplace
- Rankings
- Transparency
- Community
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bluffnet.gg
  spf: false
hosts:
- cert_expires: Jan 12 08:34:55 2027 GMT
  host: bluffnet.gg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bluffnet Gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BluffNet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: BluffNet
provider_slug: bluffnet-gg
slug: bluffnet-gg-domain-security
source_filename: bluffnet-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluffnet.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:34:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bluffnet.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bluffnet-gg/security/bluffnet-gg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Gaming
- Poker
- Platform
---

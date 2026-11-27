---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docteurbet.fr
  spf: true
hosts:
- cert_expires: Dec  7 19:56:09 2026 GMT
  host: docteurbet.fr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docteur Bet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docteur Bet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Docteur Bet
provider_slug: docteurbet-fr
slug: docteurbet-fr-domain-security
source_filename: docteurbet-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docteurbet.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 19:56:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: docteurbet.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/docteurbet-fr/security/docteurbet-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Value betting
- Sports Betting
- Subscription Service
- Odds Comparison
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryrisotto.com
  spf: true
hosts:
- cert_expires: Jan 17 20:42:44 2027 GMT
  host: tryrisotto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Risotto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Risotto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Risotto
provider_slug: risotto
slug: risotto-domain-security
source_filename: risotto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryrisotto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 20:42:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tryrisotto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/risotto/security/risotto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- HelpDesk
- ITAutomation
- Ticketing
---

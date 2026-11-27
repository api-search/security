---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ayebot.com
  spf: true
hosts:
- cert_expires: Jan  8 10:37:53 2027 GMT
  host: ayebot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ayebot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ayebot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Ayebot
provider_slug: ayebot-com
slug: ayebot-com-domain-security
source_filename: ayebot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ayebot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 10:37:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ayebot.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ayebot-com/security/ayebot-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- AI-powered business broker
- M&A
- Singapore
- Southeast Asia
- Business Valuation
- Exit Readiness
---

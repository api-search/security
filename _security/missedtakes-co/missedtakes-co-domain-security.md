---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: missedtakes.co
  spf: true
hosts:
- cert_expires: Dec 28 11:08:39 2026 GMT
  host: missedtakes.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MissedTakes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MissedTakes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MissedTakes
provider_slug: missedtakes-co
slug: missedtakes-co-domain-security
source_filename: missedtakes-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: missedtakes.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 11:08:39 2026 GMT\n  hsts: null\ndomains:\n- domain: missedtakes.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/missedtakes-co/security/missedtakes-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Platform
- Predictions
- Sports
- Politics
- Economics
---

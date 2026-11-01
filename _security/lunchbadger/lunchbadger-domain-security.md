---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunchbadger.com
  spf: true
hosts:
- cert_expires: Dec 26 20:59:36 2026 GMT
  host: www.lunchbadger.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lunchbadger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LunchBadger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LunchBadger
provider_slug: lunchbadger
slug: lunchbadger-domain-security
source_filename: lunchbadger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lunchbadger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:59:36 2026 GMT\n  hsts: null\ndomains:\n- domain: lunchbadger.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lunchbadger/security/lunchbadger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API-Design
- Low-Code
- Microservices
- Enterprise
---

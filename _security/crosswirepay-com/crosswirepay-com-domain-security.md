---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: crosswirepay.com
  spf: false
hosts:
- cert_expires: Jan 26 17:52:44 2027 GMT
  host: crosswirepay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crosswirepay Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crosswire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Crosswire
provider_slug: crosswirepay-com
slug: crosswirepay-com-domain-security
source_filename: crosswirepay-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crosswirepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 17:52:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crosswirepay.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crosswirepay-com/security/crosswirepay-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Banking
- Payments
---

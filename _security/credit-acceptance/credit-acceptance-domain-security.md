---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: creditacceptance.com
  spf: true
hosts:
- cert_expires: Jan 27 01:11:25 2027 GMT
  host: creditacceptance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credit Acceptance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credit Acceptance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Credit Acceptance
provider_slug: credit-acceptance
slug: credit-acceptance-domain-security
source_filename: credit-acceptance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creditacceptance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 01:11:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: creditacceptance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/credit-acceptance/security/credit-acceptance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Auto
- Subprime
- Lending
- Dealers
---

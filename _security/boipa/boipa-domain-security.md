---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boipa.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: boipa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BOI Payment Acceptance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BOI Payment Acceptance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BOI Payment Acceptance
provider_slug: boipa
slug: boipa-domain-security
source_filename: boipa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boipa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: boipa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/boipa/security/boipa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Card Processing
- Ireland
- B2B
- Financial Services
---

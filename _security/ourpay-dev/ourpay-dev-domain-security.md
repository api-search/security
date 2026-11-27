---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ourpay.dev
  spf: true
hosts:
- cert_expires: Feb 11 08:01:21 2027 GMT
  host: ourpay.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ourpay-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ourpay-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ourpay-dev
provider_slug: ourpay-dev
slug: ourpay-dev-domain-security
source_filename: ourpay-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ourpay.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 08:01:21 2027 GMT\n  hsts: null\ndomains:\n- domain: ourpay.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ourpay-dev/security/ourpay-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Fintech
- Developer Tools
- PaymentsPlatform
---

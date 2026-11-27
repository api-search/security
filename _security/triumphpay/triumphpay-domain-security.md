---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: triumphpay.com
  spf: true
hosts:
- cert_expires: Jan 20 10:02:46 2027 GMT
  host: triumphpay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Triumph Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triumph Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Triumph Network
provider_slug: triumphpay
slug: triumphpay-domain-security
source_filename: triumphpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triumphpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 10:02:46 2027 GMT\n  hsts: false\ndomains:\n- domain: triumphpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/triumphpay/security/triumphpay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Factoring
- Carrier Solutions
- Equipment Financing
- Insurance
- Fuel Card
- TBK Bank
---

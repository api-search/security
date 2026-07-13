---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novopayment.com
  spf: true
hosts:
- cert_expires: Oct  4 04:37:21 2026 GMT
  host: developer.novopayment.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novopayment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NovoPayment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NovoPayment
provider_slug: novopayment
slug: novopayment-domain-security
source_filename: novopayment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.novopayment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:37:21 2026 GMT\n  hsts: false\ndomains:\n- domain: novopayment.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/security/novopayment-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fraud.net
  spf: true
hosts:
- cert_expires: Sep 20 06:09:56 2026 GMT
  host: fraud.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 10:02:03 2026 GMT
  host: api-docs.fraud.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fraud Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fraud.net, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fraud.net
provider_slug: fraud-net
slug: fraud-net-domain-security
source_filename: fraud-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fraud.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:09:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.fraud.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fraud.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fraud-net/refs/heads/main/security/fraud-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud
- Risk
- Commerce
- Payments
- Security
---

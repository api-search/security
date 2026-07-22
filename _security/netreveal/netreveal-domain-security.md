---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: baesystems.com
  spf: true
hosts:
- cert_expires: Oct  7 12:44:41 2026 GMT
  host: www.baesystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netreveal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netreveal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Netreveal
provider_slug: netreveal
slug: netreveal-domain-security
source_filename: netreveal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baesystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:44:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: baesystems.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netreveal/refs/heads/main/security/netreveal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AML
- Compliance
- Financial Crime
- Fraud Detection
- Risk Management
- Sanctions Screening
---

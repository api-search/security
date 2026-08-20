---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bankunited.com
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: www.bankunited.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: developer.bankunited.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Bankunited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BankUnited, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BankUnited
provider_slug: bankunited
slug: bankunited-domain-security
source_filename: bankunited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankunited.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bankunited.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: bankunited.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankunited/refs/heads/main/security/bankunited-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Regional Bank
- Commercial Banking
- Open Finance
- Developer Portal
---

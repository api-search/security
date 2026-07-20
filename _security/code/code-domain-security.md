---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getcode.com
  spf: true
hosts:
- host: getcode.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''getcode.com'
kind: domain-security
layout: security
method: probed
name: Code Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Code
provider_slug: code
slug: code-domain-security
source_filename: code-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcode.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''getcode.com'\n  hsts: null\ndomains:\n- domain: getcode.com\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code/refs/heads/main/security/code-domain-security.yml
summary_line: DMARC
tags:
- Company
- Payments
- Micropayments
- Wallet
- Solana
- Blockchain
- Cryptocurrency
- gRPC
- Self-Custodial
---

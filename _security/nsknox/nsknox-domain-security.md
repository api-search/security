---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nsknox.net
  spf: true
hosts:
- cert_expires: Oct 20 07:54:00 2026 GMT
  host: nsknox.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nsknox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nsKnox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: nsKnox
provider_slug: nsknox
slug: nsknox-domain-security
source_filename: nsknox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nsknox.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 07:54:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nsknox.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nsknox/refs/heads/main/security/nsknox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Fraud
- Financial-Services
- Banking
- Security
- Fraud Prevention
- Bank Account Validation
- Accounts Payable
- Accounts Receivable
- Fintech
- Compliance
- Israel
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: verituity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: verituityplatform.com
  spf: true
hosts:
- cert_expires: Nov 12 06:44:20 2026 GMT
  host: verituity.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 20:24:08 2026 GMT
  host: platform.dev.verituityplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verituity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verituity, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Verituity
provider_slug: verituity
slug: verituity-domain-security
source_filename: verituity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verituity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 06:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: platform.dev.verituityplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 20:24:08 2026 GMT\n  hsts: null\ndomains:\n- domain: verituity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: verituityplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verituity/refs/heads/main/security/verituity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payouts
- Disbursements
- Identity Verification
- Account Verification
- Fraud Prevention
- Payment Integrity
- Banking
- Financial Services
- Public Sector
- ISO 20022
- Compliance
- Company
---

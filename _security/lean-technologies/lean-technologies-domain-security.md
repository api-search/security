---
api_specs:
- filename: lean-technologies-account-on-file-openapi.yml
  format: yaml
  label: Lean UAE Open Finance & Payments
  slug: lean-uae-open-finance-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-account-on-file-openapi.yml
- filename: lean-technologies-ksa-accounts-access-consents-openapi.yml
  format: yaml
  label: Lean KSA Open Banking
  slug: lean-ksa-open-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leantech.me
  spf: true
hosts:
- cert_expires: Oct  7 21:16:35 2026 GMT
  host: sandbox.leantech.me
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 05:16:48 2026 GMT
  host: api2.leantech.me
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.sandbox.sa.leantech.me
  https: false
kind: domain-security
layout: security
method: probed
name: Lean Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lean Technologies, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lean Technologies
provider_slug: lean-technologies
slug: lean-technologies-domain-security
source_filename: lean-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sandbox.leantech.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:16:35 2026 GMT\n  hsts: null\n- host: api2.leantech.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 05:16:48 2026 GMT\n  hsts: null\n- host: api.sandbox.sa.leantech.me\n  https: false\ndomains:\n- domain: leantech.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/security/lean-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Banking
- Open Finance
- Payments
- Financial Data
- Fintech
- MENA
- UAE
- Saudi Arabia
- Pay by Bank
- Bank Data
- Account Verification
- Payouts
---

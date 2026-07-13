---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atomic.financial
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atomicfi.com
  spf: true
hosts:
- cert_expires: Aug 25 11:53:54 2026 GMT
  host: atomic.financial
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: console.atomicfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: docs.atomicfi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atomic Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Atomic
provider_slug: atomic-financial
slug: atomic-financial-domain-security
source_filename: atomic-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomic.financial\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:53:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.atomicfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.atomicfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: atomic.financial\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atomicfi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-financial/refs/heads/main/security/atomic-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Income
- Payroll
- Direct Deposit
- Employment Verification
- Open Banking
- Financial
- Subscriptions
- Bill Pay
---

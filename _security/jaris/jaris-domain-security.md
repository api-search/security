---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@jaris.io"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jaris.io
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: jaris.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jaris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jaris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jaris
provider_slug: jaris
slug: jaris-domain-security
source_filename: jaris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jaris.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jaris.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@jaris.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaris/refs/heads/main/security/jaris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Embedded Finance
- Fintech
- Payments
- Lending
- Banking as a Service
- Instant Payouts
- Merchant Onboarding
- KYB
- Settlements
---

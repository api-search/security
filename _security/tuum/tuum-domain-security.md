---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tuum.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tuumplatform.com
  spf: true
hosts:
- cert_expires: Sep  6 15:19:59 2026 GMT
  host: tuum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: developer.tuumplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: auth-api.sandbox.tuumplatform.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tuum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuum, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tuum
provider_slug: tuum
slug: tuum-domain-security
source_filename: tuum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tuum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:19:59 2026 GMT\n  hsts: false\n- host: developer.tuumplatform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\n- host: auth-api.sandbox.tuumplatform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tuum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tuumplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuum/refs/heads/main/security/tuum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Core Banking
- Banking as a Service
- Payments
- Lending
- Cards
- Fintech
- Financial Services
- API
---

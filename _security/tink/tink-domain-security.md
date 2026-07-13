---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "multicert.com"
  - 0 iodef "mailto:security@tink.se"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "e-szigno.hu"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tink.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: tink.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: docs.tink.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.tink.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tink, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tink
provider_slug: tink
slug: tink-domain-security
source_filename: tink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: docs.tink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.tink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tink.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"multicert.com\"\n  - 0 iodef \"mailto:security@tink.se\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"e-szigno.hu\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tink/refs/heads/main/security/tink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Open Banking
- PSD2
- Europe
- Visa
- Account Aggregation
- Payments
- KYC
---

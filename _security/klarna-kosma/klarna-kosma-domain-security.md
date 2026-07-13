---
description: ''
domains:
- caa:
  - 0 issue "quovadisglobal.com"
  - 0 issue "e-szigno.hu"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klarna.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.klarna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: docs.openbanking.klarna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.openbanking.klarna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klarna Kosma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klarna Kosma, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Klarna Kosma
provider_slug: klarna-kosma
slug: klarna-kosma-domain-security
source_filename: klarna-kosma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klarna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openbanking.klarna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\n- host: api.openbanking.klarna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: klarna.com\n  dnssec: false\n  caa:\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"e-szigno.hu\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarna-kosma/refs/heads/main/security/klarna-kosma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Banking
- PSD2
- AIS
- PIS
- Account Information
- Payment Initiation
- KYC
- Identity Verification
- Categorization
- Insights
- Embedded Finance
- BNPL
- Lending
- Fintech
- Banking
---

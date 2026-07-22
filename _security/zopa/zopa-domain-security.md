---
api_specs:
- filename: zopa-account-info-openapi-original.yml
  format: yaml
  label: Zopa Account & Transaction API (AIS)
  slug: zopa-account-info
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-account-info-openapi-original.yml
- filename: zopa-payment-initiation-openapi-original.yml
  format: yaml
  label: Zopa Payment Initiation API (PIS)
  slug: zopa-payment-initiation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-payment-initiation-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zopa.com
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: www.zopa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zopa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zopa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: zopa
provider_slug: zopa
slug: zopa-domain-security
source_filename: zopa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zopa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zopa.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/security/zopa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Banking
- Fintech
- Open Banking
- PSD2
- Payments
- Account Information
- Payment Initiation
- FAPI
- United Kingdom
- Digital Bank
- Lending
---

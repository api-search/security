---
api_specs:
- filename: revolut-business-openapi.yaml
  format: yaml
  label: Revolut Business API
  slug: revolut-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-business-openapi.yaml
- filename: revolut-merchant-openapi.yaml
  format: yaml
  label: Revolut Merchant API
  slug: revolut-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-merchant-openapi.yaml
- filename: revolut-open-banking-openapi.yaml
  format: yaml
  label: Revolut Open Banking API
  slug: revolut-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-open-banking-openapi.yaml
- filename: revolut-crypto-ramp-openapi.yaml
  format: yaml
  label: Revolut Crypto Ramp API
  slug: revolut-crypto-ramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-crypto-ramp-openapi.yaml
- filename: revolut-x-openapi.yaml
  format: yaml
  label: Revolut X API
  slug: revolut-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/openapi/revolut-x-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seedcamp.com
  spf: true
- caa:
  - 0 iodef "mailto:security@revolut.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "buypass.com"
  - 0 issue "visa.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revolut.com
  spf: true
hosts:
- cert_expires: Oct  5 21:34:34 2026 GMT
  host: seedcamp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: b2b.revolut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: sandbox-b2b.revolut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revolut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revolut, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revolut
provider_slug: revolut
slug: revolut-domain-security
source_filename: revolut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seedcamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:34:34 2026 GMT\n  hsts: false\n- host: b2b.revolut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox-b2b.revolut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: seedcamp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: revolut.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@revolut.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"buypass.com\"\n  - 0 issue \"visa.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolut/refs/heads/main/security/revolut-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Banking
- Open Banking
- Merchant Acquiring
- Cryptocurrency
- Cards
---

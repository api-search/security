---
api_specs:
- filename: backbase-approve-api-openapi.yml
  format: yaml
  label: BackBase Approve API
  slug: backbase-approve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-approve-api-openapi.yml
- filename: backbase-bbt-api-openapi.yml
  format: yaml
  label: BackBase Bbt API
  slug: backbase-bbt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-bbt-api-openapi.yml
- filename: backbase-patch-api-openapi.yml
  format: yaml
  label: BackBase Patch API
  slug: backbase-patch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-patch-api-openapi.yml
- filename: backbase-payment-orders-api-openapi.yml
  format: yaml
  label: BackBase Payment Orders API
  slug: backbase-payment-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-payment-orders-api-openapi.yml
- filename: backbase-test-api-openapi.yml
  format: yaml
  label: BackBase Test API
  slug: backbase-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-test-api-openapi.yml
- filename: backbase-utility-api-openapi.yml
  format: yaml
  label: BackBase Utility API
  slug: backbase-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-utility-api-openapi.yml
- filename: backbase-validate-api-openapi.yml
  format: yaml
  label: BackBase Validate API
  slug: backbase-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-validate-api-openapi.yml
- filename: backbase-wallet-api-openapi.yml
  format: yaml
  label: BackBase Wallet API
  slug: backbase-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-wallet-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa@backbase.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backbase.com
  spf: true
hosts:
- cert_expires: Nov 25 14:21:40 2026 GMT
  host: www.backbase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Backbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BackBase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BackBase
provider_slug: backbase
slug: backbase-domain-security
source_filename: backbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.backbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 14:21:40 2026 GMT\n  hsts: false\ndomains:\n- domain: backbase.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa@backbase.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/security/backbase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- Fintech
- Digital Banking
- API Platform
- AI-Native
---

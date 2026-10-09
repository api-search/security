---
api_specs:
- filename: centrapay-payment-requests-api-openapi.yml
  format: yaml
  label: Centrapay Payment Requests API
  slug: centrapay-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/openapi/centrapay-payment-requests-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:alerts@centrapay.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centrapay.com
  spf: true
hosts:
- cert_expires: Dec 14 00:36:39 2026 GMT
  host: centrapay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centrapay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centrapay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Centrapay
provider_slug: centrapay
slug: centrapay-domain-security
source_filename: centrapay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centrapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 00:36:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: centrapay.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:alerts@centrapay.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/security/centrapay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Digital Wallets
- Open Banking
- QR Code Payments
- Loyalty
- Gift Cards
- Fintech
---

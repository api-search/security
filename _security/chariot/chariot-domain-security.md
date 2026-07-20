---
api_specs:
- filename: chariot-openapi-original.yml
  format: yaml
  label: Chariot API
  slug: chariot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/openapi/chariot-openapi-original.yml
- filename: chariot-fdx-openapi-original.yml
  format: yaml
  label: Chariot FDX API
  slug: chariot-fdx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/openapi/chariot-fdx-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: givechariot.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: api.givechariot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: devapi.givechariot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: sandboxapi.givechariot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chariot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chariot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chariot
provider_slug: chariot
slug: chariot-domain-security
source_filename: chariot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.givechariot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: null\n- host: devapi.givechariot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: null\n- host: sandboxapi.givechariot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: givechariot.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/security/chariot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Donor Advised Funds
- Charitable Giving
- Nonprofit
- Fintech
- DAFpay
- Grants
- Disbursements
- Open Banking
- FDX
- Webhooks
- Company
---

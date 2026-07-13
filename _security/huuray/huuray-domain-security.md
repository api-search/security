---
api_specs:
- filename: huuray-openapi.yml
  format: yaml
  label: Huuray Gift Card API
  slug: huuray-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huuray/refs/heads/main/openapi/huuray-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:sslreports@onlinedata.dk"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: huuray.com
  spf: true
hosts:
- cert_expires: Oct  8 00:10:51 2026 GMT
  host: huuray.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 04:27:21 2026 GMT
  host: api.huuray.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Huuray Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huuray, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Huuray
provider_slug: huuray
slug: huuray-domain-security
source_filename: huuray-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huuray.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:10:51 2026 GMT\n  hsts: false\n- host: api.huuray.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  7 04:27:21 2026 GMT\n  hsts: null\ndomains:\n- domain: huuray.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:sslreports@onlinedata.dk\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huuray/refs/heads/main/security/huuray-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Gift Cards
- Payments
- Rewards
---

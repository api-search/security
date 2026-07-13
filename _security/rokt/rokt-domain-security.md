---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Rokt Query API
  slug: rokt-query-api
  spec_type: OpenAPI
  url: https://docs.rokt.com/openapi/
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:infosec@rokt.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rokt.com
  spf: true
hosts:
- cert_expires: Sep 29 00:12:59 2026 GMT
  host: www.rokt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 07:43:53 2026 GMT
  host: docs.rokt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.rokt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rokt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rokt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rokt
provider_slug: rokt
slug: rokt-domain-security
source_filename: rokt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rokt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:12:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rokt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:43:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rokt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rokt.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:infosec@rokt.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rokt/refs/heads/main/security/rokt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- Advertising
- Transaction Moment
- Personalization
- Offers
- Analytics
- Reporting
---

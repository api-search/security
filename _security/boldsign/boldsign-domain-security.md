---
api_specs:
- filename: index.html
  format: yaml
  label: BoldSign eSignature API
  slug: boldsign-esignature-api
  spec_type: OpenAPI
  url: https://api.boldsign.com/swagger/index.html
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: boldsign.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: boldsign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: developers.boldsign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.boldsign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boldsign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoldSign, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BoldSign
provider_slug: boldsign
slug: boldsign-domain-security
source_filename: boldsign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boldsign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.boldsign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.boldsign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: boldsign.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/security/boldsign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Signature
- Electronic Signature
- Document Management
- Embedded Signing
- Webhooks
- Templates
- Identity Verification
- Compliance
---

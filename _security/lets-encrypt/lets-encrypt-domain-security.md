---
api_specs:
- filename: lets-encrypt-acme-openapi.yml
  format: yaml
  label: Let's Encrypt ACME API
  slug: lets-encrypt-acme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lets-encrypt/refs/heads/main/openapi/lets-encrypt-acme-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "www.digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: letsencrypt.org
  spf: true
hosts:
- cert_expires: Oct  4 15:24:33 2026 GMT
  host: letsencrypt.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 23:05:30 2026 GMT
  host: acme-v02.api.letsencrypt.org
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 21:57:59 2026 GMT
  host: acme-staging-v02.api.letsencrypt.org
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lets Encrypt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Let''s Encrypt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Let's Encrypt
provider_slug: lets-encrypt
slug: lets-encrypt-domain-security
source_filename: lets-encrypt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letsencrypt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:24:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: acme-v02.api.letsencrypt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:05:30 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: acme-staging-v02.api.letsencrypt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:57:59 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: letsencrypt.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lets-encrypt/refs/heads/main/security/lets-encrypt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Certificates
- Linux Foundation
- Security
- TLS
- ACME
- PKI
---

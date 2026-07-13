---
api_specs:
- filename: duo-admin-api-openapi.yml
  format: yaml
  label: Duo Admin API
  slug: duo-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-admin-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "identrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: duo.com
  spf: true
- caa:
  - 0 issue "identrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: duosecurity.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: duo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api-xxxxxxxx.duosecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duo Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duo Security, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Duo Security
provider_slug: duo-security
slug: duo-security-domain-security
source_filename: duo-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-xxxxxxxx.duosecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: duo.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: duosecurity.com\n  dnssec: false\n  caa:\n  - 0 issue \"identrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/security/duo-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- MFA
- Zero Trust
- Identity
---

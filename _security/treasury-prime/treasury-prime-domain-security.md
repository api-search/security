---
api_specs:
- filename: treasury-prime-openapi.yml
  format: yaml
  label: Treasury Prime Bank API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/openapi/treasury-prime-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: treasuryprime.com
  spf: true
hosts:
- cert_expires: Oct  9 18:07:15 2026 GMT
  host: www.treasuryprime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developers.treasuryprime.com
  https: false
- host: sandbox.treasuryprime.com
  https: false
kind: domain-security
layout: security
method: probed
name: Treasury Prime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treasury Prime, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Treasury Prime
provider_slug: treasury-prime
slug: treasury-prime-domain-security
source_filename: treasury-prime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treasuryprime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 18:07:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.treasuryprime.com\n  https: false\n- host: sandbox.treasuryprime.com\n  https: false\ndomains:\n- domain: treasuryprime.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasury-prime/refs/heads/main/security/treasury-prime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
---

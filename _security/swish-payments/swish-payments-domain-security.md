---
api_specs:
- filename: swish-payments-openapi-generated.yml
  format: yaml
  label: Swish API
  slug: swish-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swish-payments/openapi/_ae-authored/swish-payments-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:domain@getswish.se"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: swish.nu
  spf: true
hosts:
- cert_expires: Feb  2 20:28:08 2027 GMT
  host: swish.nu
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Swish
provider_slug: swish-payments
slug: swish-payments-domain-security
source_filename: swish-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swish.nu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 20:28:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: swish.nu\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:domain@getswish.se\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/swish-payments/security/swish-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Mobile
- Fintech
- Sweden
- Person-to-Person
---

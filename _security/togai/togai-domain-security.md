---
api_specs:
- filename: togai-openapi.yml
  format: yaml
  label: Togai API
  slug: togai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/togai/refs/heads/main/openapi/togai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:engg-togai@zuora.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: togai.com
  spf: true
hosts:
- cert_expires: Aug 29 03:09:36 2026 GMT
  host: www.togai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 22:53:44 2026 GMT
  host: docs.togai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.togai.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Togai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Togai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Togai
provider_slug: togai
slug: togai-domain-security
source_filename: togai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.togai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 03:09:36 2026 GMT\n  hsts: false\n- host: docs.togai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:53:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.togai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: togai.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:engg-togai@zuora.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/togai/refs/heads/main/security/togai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Metering
- Usage-Based Pricing
- Revenue Management
- SaaS
- Fintech
---

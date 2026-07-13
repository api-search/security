---
api_specs:
- filename: zapier-partner-api.yml
  format: yaml
  label: Zapier Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-partner-api.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zapier.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: zapier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.zapier.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: actions.zapier.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zapier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zapier, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zapier
provider_slug: zapier
slug: zapier-domain-security
source_filename: zapier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zapier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zapier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\n- host: actions.zapier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zapier.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/security/zapier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integrations
- iPaaS
---

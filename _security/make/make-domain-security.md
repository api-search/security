---
api_specs:
- filename: make-openapi.yml
  format: yaml
  label: Make API
  slug: make-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/make/refs/heads/main/openapi/make-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: make.com
  spf: true
hosts:
- cert_expires: Sep 23 11:23:17 2026 GMT
  host: developers.make.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:14:34 2026 GMT
  host: us1.make.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:14:38 2026 GMT
  host: us2.make.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Make Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Make, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Make
provider_slug: make
slug: make-domain-security
source_filename: make-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.make.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:23:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us1.make.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:14:34 2026 GMT\n  hsts: null\n- host: us2.make.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:14:38 2026 GMT\n  hsts: null\ndomains:\n- domain: make.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/make/refs/heads/main/security/make-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Integration
- iPaaS
- No-Code
- Scenarios
- Workflows
---

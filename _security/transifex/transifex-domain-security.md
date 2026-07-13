---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Transifex API
  slug: transifex-api
  spec_type: OpenAPI
  url: https://transifex.github.io/openapi/
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@transifex.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transifex.com
  spf: true
hosts:
- cert_expires: Oct  2 11:33:08 2026 GMT
  host: www.transifex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:46:33 2026 GMT
  host: developers.transifex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: rest.api.transifex.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transifex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transifex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Transifex
provider_slug: transifex
slug: transifex-domain-security
source_filename: transifex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transifex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:33:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.transifex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:46:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.api.transifex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: transifex.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@transifex.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transifex/refs/heads/main/security/transifex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Localization
- Translation
- i18n
- l10n
- Language
- Content Management
- Workflow Automation
---

---
api_specs:
- filename: agave-unified-api-openapi.yml
  format: yaml
  label: Agave Unified Construction API
  slug: unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-unified-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agaveapi.com
  spf: true
hosts:
- cert_expires: Sep 29 19:34:51 2026 GMT
  host: docs.agaveapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.agaveapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: sandbox.agaveapi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Agave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agave, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agave
provider_slug: agave
slug: agave-domain-security
source_filename: agave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.agaveapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:34:51 2026 GMT\n  hsts: false\n- host: api.agaveapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.agaveapi.com\n  https: false\ndomains:\n- domain: agaveapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/security/agave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accounting
- Construction
- Integration
---

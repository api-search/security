---
api_specs:
- filename: integry-openapi.yml
  format: yaml
  label: Integry API
  slug: apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integry/refs/heads/main/openapi/integry-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: integry.io
  spf: true
hosts:
- host: integry.io
  https: false
- cert_expires: Sep  7 05:02:16 2026 GMT
  host: api.integry.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Integry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Integry, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Integry
provider_slug: integry
slug: integry-domain-security
source_filename: integry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: integry.io\n  https: false\n- host: api.integry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 05:02:16 2026 GMT\n  hsts: null\ndomains:\n- domain: integry.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integry/refs/heads/main/security/integry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Embedded iPaaS
- Integration
- Native Integrations
---

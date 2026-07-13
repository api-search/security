---
api_specs:
- filename: stackone-openapi.yml
  format: yaml
  label: StackOne
  slug: stackone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackone/refs/heads/main/openapi/stackone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stackone.com
  spf: true
hosts:
- cert_expires: Sep 20 20:25:02 2026 GMT
  host: www.stackone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 22:55:25 2026 GMT
  host: docs.stackone.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: api.stackone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stackone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackOne, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: StackOne
provider_slug: stackone
slug: stackone-domain-security
source_filename: stackone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stackone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:25:02 2026 GMT\n  hsts: false\n- host: docs.stackone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:55:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.stackone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stackone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackone/refs/heads/main/security/stackone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integrations
- iPaaS
---

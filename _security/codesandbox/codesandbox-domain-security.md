---
api_specs:
- filename: codesandbox-sdk-openapi.yml
  format: yaml
  label: CodeSandbox SDK API
  slug: sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/openapi/codesandbox-sdk-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codesandbox.io
  spf: true
hosts:
- cert_expires: Sep 26 16:44:57 2026 GMT
  host: codesandbox.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:44:26 2026 GMT
  host: api.codesandbox.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:44:26 2026 GMT
  host: sandpack.codesandbox.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codesandbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeSandbox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CodeSandbox
provider_slug: codesandbox
slug: codesandbox-domain-security
source_filename: codesandbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codesandbox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:44:57 2026 GMT\n  hsts: false\n- host: api.codesandbox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:44:26 2026 GMT\n  hsts: false\n- host: sandpack.codesandbox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:44:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codesandbox.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesandbox/refs/heads/main/security/codesandbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Cloud IDE
- Code Sandboxes
- Browser Development
- AI Sandboxes
- Code Embedding
---

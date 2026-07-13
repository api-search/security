---
api_specs:
- filename: fly-io-machines-api-openapi.yml
  format: yaml
  label: Fly.io Machines API
  slug: machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fly-io/refs/heads/main/openapi/fly-io-machines-api-openapi.yml
- filename: fly-io-extensions-api-openapi.yml
  format: yaml
  label: Fly.io Extensions API
  slug: extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fly-io/refs/heads/main/openapi/fly-io-extensions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fly.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: machines.dev
  spf: false
hosts:
- cert_expires: Oct  2 11:21:26 2026 GMT
  host: fly.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:27:35 2026 GMT
  host: api.machines.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 11:20:50 2026 GMT
  host: api.fly.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fly Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fly-io, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: fly-io
provider_slug: fly-io
slug: fly-io-domain-security
source_filename: fly-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:21:26 2026 GMT\n  hsts: false\n- host: api.machines.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:27:35 2026 GMT\n  hsts: null\n- host: api.fly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 11:20:50 2026 GMT\n  hsts: null\ndomains:\n- domain: fly.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: machines.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fly-io/refs/heads/main/security/fly-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---

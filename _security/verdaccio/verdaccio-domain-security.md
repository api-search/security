---
api_specs:
- filename: verdaccio-npm-registry-api-openapi.yml
  format: yaml
  label: Verdaccio npm Registry API
  slug: verdaccio-npm-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/openapi/verdaccio-npm-registry-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: verdaccio.org
  spf: true
hosts:
- cert_expires: Sep  3 08:05:21 2026 GMT
  host: www.verdaccio.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verdaccio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verdaccio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Verdaccio
provider_slug: verdaccio
slug: verdaccio-domain-security
source_filename: verdaccio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verdaccio.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 08:05:21 2026 GMT\n  hsts: false\ndomains:\n- domain: verdaccio.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdaccio/refs/heads/main/security/verdaccio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- npm
- registry
- package-manager
- private-registry
- proxy
- nodejs
- open-source
- self-hosted
- yarn
- pnpm
- docker
- kubernetes
---

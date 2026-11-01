---
api_specs:
- filename: seekrit-dev-docs-openapi-generated.yml
  format: yaml
  label: seekrit-dev docs API
  slug: docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/seekrit-dev/openapi/_ae-authored/seekrit-dev-docs-openapi-generated.yml
- filename: seekrit-dev-guides-openapi-generated.yml
  format: yaml
  label: seekrit-dev guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/seekrit-dev/openapi/_ae-authored/seekrit-dev-guides-openapi-generated.yml
- filename: seekrit-dev-reference-openapi-generated.yml
  format: yaml
  label: seekrit-dev reference API
  slug: reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/seekrit-dev/openapi/_ae-authored/seekrit-dev-reference-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seekrit.dev
  spf: true
hosts:
- cert_expires: Jan 27 05:21:27 2027 GMT
  host: seekrit.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seekrit Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for seekrit-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: seekrit-dev
provider_slug: seekrit-dev
slug: seekrit-dev-domain-security
source_filename: seekrit-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seekrit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 05:21:27 2027 GMT\n  hsts: false\ndomains:\n- domain: seekrit.dev\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/seekrit-dev/security/seekrit-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Secrets Management
- Encryption
- Cloudflare
---

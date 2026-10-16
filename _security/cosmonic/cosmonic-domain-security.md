---
api_specs:
- filename: cosmonic-core-openapi-generated.yml
  format: yaml
  label: Cosmonic core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmonic/refs/heads/main/openapi/_ae-authored/cosmonic-core-openapi-generated.yml
- filename: cosmonic-desktop-openapi-generated.yml
  format: yaml
  label: Cosmonic Get Started API
  slug: desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmonic/refs/heads/main/openapi/_ae-authored/cosmonic-desktop-openapi-generated.yml
- filename: cosmonic-template-catalog-openapi-generated.yml
  format: yaml
  label: Cosmonic Template Catalog API
  slug: template-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmonic/refs/heads/main/openapi/_ae-authored/cosmonic-template-catalog-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosmonic.com
  spf: true
hosts:
- cert_expires: Dec 26 17:23:59 2026 GMT
  host: cosmonic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosmonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cosmonic
provider_slug: cosmonic
slug: cosmonic-domain-security
source_filename: cosmonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cosmonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 17:23:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cosmonic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmonic/refs/heads/main/security/cosmonic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Sandbox
- Cloud
- Platform
- Wasm
---

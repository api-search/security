---
api_specs:
- filename: buildpacks-io-buildpacks-api-openapi.yml
  format: yaml
  label: buildpacks-io Buildpacks API
  slug: buildpacks-io-buildpacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildpacks-io/refs/heads/main/openapi/buildpacks-io-buildpacks-api-openapi.yml
- filename: buildpacks-io-search-api-openapi.yml
  format: yaml
  label: buildpacks-io Search API
  slug: buildpacks-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildpacks-io/refs/heads/main/openapi/buildpacks-io-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: buildpacks.io
  spf: false
hosts:
- cert_expires: Nov 28 16:40:17 2026 GMT
  host: www.buildpacks.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 16:40:17 2026 GMT
  host: buildpacks.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 00:36:08 2026 GMT
  host: registry.buildpacks.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Buildpacks Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildpacks Io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Buildpacks Io
provider_slug: buildpacks-io
slug: buildpacks-io-domain-security
source_filename: buildpacks-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buildpacks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: buildpacks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: registry.buildpacks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 00:36:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: buildpacks.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildpacks-io/refs/heads/main/security/buildpacks-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native Buildpacks
- Container Images
- Build Automation
- CNCF
- Open Source
- Developer Tools
- OCI
- Specification
- Supply Chain
- Registry
---

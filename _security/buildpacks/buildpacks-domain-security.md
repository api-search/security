---
api_specs:
- filename: buildpacks-kpack-swagger.json
  format: json
  label: kpack
  slug: kpack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildpacks/refs/heads/main/openapi/buildpacks-kpack-swagger.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: buildpacks.io
  spf: false
hosts:
- cert_expires: Nov 28 16:40:17 2026 GMT
  host: buildpacks.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 01:47:19 2026 GMT
  host: registry.buildpacks.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Buildpacks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud Native Buildpacks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cloud Native Buildpacks
provider_slug: buildpacks
slug: buildpacks-domain-security
source_filename: buildpacks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildpacks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: registry.buildpacks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:47:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: buildpacks.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildpacks/refs/heads/main/security/buildpacks-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Build Tools
- CI/CD
- Cloud-Native
- CNCF
- Container Images
- Containers
- OCI
- Open-Source
---

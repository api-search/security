---
api_specs:
- filename: userig-rig-api-api-openapi.yml
  format: yaml
  label: Rig API
  slug: rig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userig/openapi/userig-rig-api-api-openapi.yml
- filename: userig-openapi-generated.yml
  format: yaml
  label: Rig API
  slug: userig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userig/openapi/_ae-authored/userig-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:rich@userig.app"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: userig.app
  spf: true
hosts:
- cert_expires: Dec 30 17:31:23 2026 GMT
  host: userig.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Userig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Rig
provider_slug: userig
slug: userig-domain-security
source_filename: userig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userig.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 17:31:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: userig.app\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:rich@userig.app\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/userig/security/userig-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Development
- Mac
- Windows
- Process-Manager
---

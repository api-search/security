---
api_specs:
- filename: grabmail-io-account-api-openapi.yml
  format: yaml
  label: grabmail-io Account API
  slug: grabmail-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabmail-io/openapi/grabmail-io-account-api-openapi.yml
- filename: grabmail-io-mailbox-api-openapi.yml
  format: yaml
  label: grabmail-io Mailbox API
  slug: grabmail-io-mailbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabmail-io/openapi/grabmail-io-mailbox-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grabmail.io
  spf: true
hosts:
- cert_expires: Dec 31 17:30:09 2026 GMT
  host: grabmail.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grabmail Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for grabmail-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: grabmail-io
provider_slug: grabmail-io
slug: grabmail-io-domain-security
source_filename: grabmail-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grabmail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 17:30:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: grabmail.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/grabmail-io/security/grabmail-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Temporary
- API
- DeveloperTools
---

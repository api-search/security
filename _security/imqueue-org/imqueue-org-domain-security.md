---
api_specs:
- filename: imqueue-org-openapi-generated.yml
  format: yaml
  label: '@imqueue API'
  slug: imqueue-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imqueue-org/openapi/_ae-authored/imqueue-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: imqueue.org
  spf: false
hosts:
- cert_expires: Dec 16 02:25:49 2026 GMT
  host: imqueue.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: '@imqueue Domain Security'
name_suffix: Domain Security
overview: 'Domain security posture for @imqueue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: '@imqueue'
provider_slug: imqueue-org
slug: imqueue-org-domain-security
source_filename: imqueue-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imqueue.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 02:25:49 2026 GMT\n  hsts: false\ndomains:\n- domain: imqueue.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/imqueue-org/security/imqueue-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Messaging
- TypeScript
- Node.js
- RPC
- Queues
---

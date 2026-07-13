---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Pantheon REST API
  slug: pantheon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pantheon/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pantheon.io
  spf: true
hosts:
- cert_expires: Sep  1 17:20:44 2026 GMT
  host: pantheon.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:35:11 2026 GMT
  host: docs.pantheon.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 22:30:14 2026 GMT
  host: terminus.pantheon.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pantheon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pantheon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pantheon
provider_slug: pantheon
slug: pantheon-domain-security
source_filename: pantheon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pantheon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:20:44 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.pantheon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:35:11 2026 GMT\n  hsts: false\n- host: terminus.pantheon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:30:14 2026 GMT\n  hsts: null\ndomains:\n- domain: pantheon.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pantheon/refs/heads/main/security/pantheon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WebOps
- WordPress
- Drupal
- CMS
- Hosting
- CDN
- DevOps
- Deployments
- Sites
- Environments
---

---
api_specs:
- filename: woodpecker-ci-server-swagger.json
  format: json
  label: Woodpecker CI Server API
  slug: server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woodpecker-ci/refs/heads/main/openapi/woodpecker-ci-server-swagger.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: woodpecker-ci.org
  spf: false
hosts:
- cert_expires: Sep 29 18:06:52 2026 GMT
  host: woodpecker-ci.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 06:12:17 2026 GMT
  host: ci.woodpecker-ci.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Woodpecker Ci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Woodpecker CI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Woodpecker CI
provider_slug: woodpecker-ci
slug: woodpecker-ci-domain-security
source_filename: woodpecker-ci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woodpecker-ci.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:06:52 2026 GMT\n  hsts: false\n- host: ci.woodpecker-ci.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:12:17 2026 GMT\n  hsts: false\ndomains:\n- domain: woodpecker-ci.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woodpecker-ci/refs/heads/main/security/woodpecker-ci-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Continuous Integration
- Continuous Delivery
- DevOps
- Developer Tools
- Open Source
- Pipelines
- Self-Hosted
- Build Automation
- Containers
---

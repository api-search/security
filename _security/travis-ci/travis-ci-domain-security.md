---
api_specs:
- filename: travis-ci-openapi.yml
  format: yaml
  label: Travis CI REST API v3
  slug: v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/openapi/travis-ci-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: travis-ci.com
  spf: true
hosts:
- cert_expires: Sep 14 10:16:45 2026 GMT
  host: www.travis-ci.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: developer.travis-ci.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.travis-ci.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Travis Ci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travis CI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Travis CI
provider_slug: travis-ci
slug: travis-ci-domain-security
source_filename: travis-ci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travis-ci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:16:45 2026 GMT\n  hsts: false\n- host: developer.travis-ci.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.travis-ci.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: travis-ci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/security/travis-ci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- CI/CD
- Build
- Open Source
- Hosted
- GitHub
---

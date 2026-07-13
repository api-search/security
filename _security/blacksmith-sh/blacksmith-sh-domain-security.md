---
api_specs:
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith GitHub Actions Runners
  slug: github-actions-runners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith Docker Builds
  slug: docker-builds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith Cache
  slug: cache
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blacksmith.sh
  spf: true
hosts:
- cert_expires: Sep 18 07:25:39 2026 GMT
  host: www.blacksmith.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 02:15:09 2026 GMT
  host: docs.blacksmith.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 02:15:09 2026 GMT
  host: app.blacksmith.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blacksmith Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blacksmith, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blacksmith
provider_slug: blacksmith-sh
slug: blacksmith-sh-domain-security
source_filename: blacksmith-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blacksmith.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:25:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.blacksmith.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:15:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.blacksmith.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:15:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blacksmith.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/security/blacksmith-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- GitHub Actions
- Runners
- Caching
- Docker
---

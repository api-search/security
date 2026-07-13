---
api_specs:
- filename: api-integration
  format: yaml
  label: Roadmunk GraphQL API
  slug: roadmunk-graphql-api
  spec_type: OpenAPI
  url: https://www.tempo.io/products/roadmaps/api-integration
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roadmunk.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@tempo.io"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tempo.io
  spf: true
hosts:
- cert_expires: Sep  6 06:32:14 2026 GMT
  host: roadmunk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 16:51:02 2026 GMT
  host: www.tempo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: app-gateway.roadmunk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roadmunk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roadmunk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Roadmunk
provider_slug: roadmunk
slug: roadmunk-domain-security
source_filename: roadmunk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roadmunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:32:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.tempo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 16:51:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app-gateway.roadmunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: roadmunk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tempo.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@tempo.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roadmunk/refs/heads/main/security/roadmunk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Roadmapping
- GraphQL
- Roadmaps
- Project Management
- Product Management
- Feedback
- Ideas
- Milestones
- Swimlanes
- Timeline
---

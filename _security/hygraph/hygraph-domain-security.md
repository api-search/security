---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hygraph.com
  spf: true
hosts:
- cert_expires: Sep 25 07:06:52 2026 GMT
  host: hygraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 12:52:38 2026 GMT
  host: api.hygraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: management.hygraph.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hygraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hygraph, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hygraph
provider_slug: hygraph
slug: hygraph-domain-security
source_filename: hygraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hygraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:06:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hygraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:52:38 2026 GMT\n  hsts: null\n- host: management.hygraph.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hygraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hygraph/refs/heads/main/security/hygraph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- Headless CMS
- Content Management
- Content Federation
- Webhooks
- Digital Experience
---

---
api_specs:
- filename: openapi.json
  format: json
  label: Keep REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.keephq.dev/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: keephq.dev
  spf: true
hosts:
- cert_expires: Aug 18 18:47:45 2026 GMT
  host: www.keephq.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:02:59 2026 GMT
  host: docs.keephq.dev
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:02:59 2026 GMT
  host: api.keephq.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keep, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Keep
provider_slug: keep
slug: keep-domain-security
source_filename: keep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keephq.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 18:47:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.keephq.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:02:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.keephq.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:02:59 2026 GMT\n  hsts: null\ndomains:\n- domain: keephq.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keep/refs/heads/main/security/keep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AIOps
- Alerting
- Incident Management
- Observability
- Open Source
- SRE
- Workflow Automation
---

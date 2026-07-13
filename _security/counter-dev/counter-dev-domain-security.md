---
api_specs:
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Tracking / Collect API
  slug: counter-dev-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Stats / Dashboard Data API
  slug: counter-dev-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Account API
  slug: counter-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: counter.dev
  spf: true
hosts:
- cert_expires: Aug 27 17:00:23 2026 GMT
  host: counter.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:00:23 2026 GMT
  host: t.counter.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Counter Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Counter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Counter
provider_slug: counter-dev
slug: counter-dev-domain-security
source_filename: counter-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: counter.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:00:23 2026 GMT\n  hsts: false\n- host: t.counter.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:00:23 2026 GMT\n  hsts: null\ndomains:\n- domain: counter.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/security/counter-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Analytics
- Privacy
- Open Source
- Tracking
- Self-Hosted
---

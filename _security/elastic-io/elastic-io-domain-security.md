---
api_specs:
- filename: elastic-io-platform-api-openapi.yml
  format: yaml
  label: Elastic.io
  slug: elastic-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/openapi/elastic-io-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elastic.io
  spf: true
hosts:
- cert_expires: Sep 15 09:40:52 2026 GMT
  host: www.elastic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 07:50:41 2026 GMT
  host: api.elastic.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elastic Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elastic.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elastic.io
provider_slug: elastic-io
slug: elastic-io-domain-security
source_filename: elastic-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elastic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:40:52 2026 GMT\n  hsts: false\n- host: api.elastic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:50:41 2026 GMT\n  hsts: null\ndomains:\n- domain: elastic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/security/elastic-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integrations
- iPaaS
- SaaS Integration
---

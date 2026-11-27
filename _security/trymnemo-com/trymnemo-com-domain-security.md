---
api_specs:
- filename: trymnemo-com-namespace-api-openapi.yml
  format: yaml
  label: Mnemo Protocol Namespace API
  slug: trymnemo-com-namespace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymnemo-com/openapi/trymnemo-com-namespace-api-openapi.yml
- filename: trymnemo-com-objects-api-openapi.yml
  format: yaml
  label: Mnemo Protocol Objects API
  slug: trymnemo-com-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymnemo-com/openapi/trymnemo-com-objects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trymnemo.com
  spf: true
hosts:
- cert_expires: Dec 30 08:59:35 2026 GMT
  host: www.trymnemo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mnemo Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mnemo Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mnemo Protocol
provider_slug: trymnemo-com
slug: trymnemo-com-domain-security
source_filename: trymnemo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trymnemo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 08:59:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trymnemo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/trymnemo-com/security/trymnemo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Embeddings
- Verification
- Vector Provenance
- Payments
---

---
api_specs:
- filename: us-army-public-openapi.yml
  format: yaml
  label: US Army Public API
  slug: us-army-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-army/refs/heads/main/openapi/us-army-public-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: army.mil
  spf: true
hosts:
- cert_expires: Dec 20 16:48:51 2026 GMT
  host: api.army.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 16:48:51 2026 GMT
  host: www.army.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Army Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Army, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Army
provider_slug: us-army
slug: us-army-domain-security
source_filename: us-army-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.army.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 16:48:51 2026 GMT\n  hsts: null\n- host: www.army.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 16:48:51 2026 GMT\n  hsts: null\ndomains:\n- domain: army.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-army/refs/heads/main/security/us-army-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Army
- Federal Government
- Military
- Defense
- Open Data
- News
---

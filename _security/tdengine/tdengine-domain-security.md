---
api_specs:
- filename: tdengine-openapi-generated.yml
  format: yaml
  label: TDengine API
  slug: tdengine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tdengine/openapi/_ae-authored/tdengine-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tdengine.com
  spf: true
hosts:
- cert_expires: Dec 15 04:24:53 2026 GMT
  host: tdengine.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TDengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TDengine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TDengine
provider_slug: tdengine
slug: tdengine-domain-security
source_filename: tdengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tdengine.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 04:24:53 2026 GMT\n  hsts: false\ndomains:\n- domain: tdengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tdengine/security/tdengine-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Time Series Database
- Industrial IoT
- AI Platform
- Open Source
---

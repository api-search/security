---
api_specs:
- filename: crisphive-com-openapi-generated.yml
  format: yaml
  label: Crisphive API
  slug: crisphive-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crisphive-com/openapi/_ae-authored/crisphive-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crisphive.com
  spf: true
hosts:
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: crisphive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crisphive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crisphive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crisphive
provider_slug: crisphive-com
slug: crisphive-com-domain-security
source_filename: crisphive-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crisphive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crisphive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crisphive-com/security/crisphive-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Scheduling
- Field Service Management
- Dispatch
---

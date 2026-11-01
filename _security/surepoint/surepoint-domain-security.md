---
api_specs:
- filename: surepoint-openapi-generated.yml
  format: yaml
  label: SurePoint Pro API
  slug: surepoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surepoint/openapi/_ae-authored/surepoint-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: surepoint.com
  spf: true
hosts:
- cert_expires: Dec 25 21:06:38 2026 GMT
  host: surepoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Surepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SurePoint Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SurePoint Pro
provider_slug: surepoint
slug: surepoint-domain-security
source_filename: surepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: surepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 21:06:38 2026 GMT\n  hsts: false\ndomains:\n- domain: surepoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/surepoint/security/surepoint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Software
- Platform
- Services
---

---
api_specs:
- filename: hitsteps-com-openapi-generated.yml
  format: yaml
  label: Hitsteps API
  slug: hitsteps-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hitsteps-com/openapi/_ae-authored/hitsteps-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hitsteps.com
  spf: true
hosts:
- cert_expires: Jan 27 19:36:03 2027 GMT
  host: hitsteps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hitsteps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hitsteps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hitsteps
provider_slug: hitsteps-com
slug: hitsteps-com-domain-security
source_filename: hitsteps-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hitsteps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:36:03 2027 GMT\n  hsts: false\ndomains:\n- domain: hitsteps.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hitsteps-com/security/hitsteps-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Analytics
- Web
- Real-Time
- Statistics
- Marketing
---

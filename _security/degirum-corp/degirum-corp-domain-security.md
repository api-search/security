---
api_specs:
- filename: degirum-corp-openapi-generated.yml
  format: yaml
  label: DeGirum Corp API
  slug: degirum-corp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/degirum-corp/openapi/_ae-authored/degirum-corp-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: degirum.com
  spf: true
hosts:
- cert_expires: Dec 29 00:00:52 2026 GMT
  host: degirum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Degirum Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeGirum Corp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeGirum Corp
provider_slug: degirum-corp
slug: degirum-corp-domain-security
source_filename: degirum-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: degirum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 00:00:52 2026 GMT\n  hsts: false\ndomains:\n- domain: degirum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/degirum-corp/security/degirum-corp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Development Tools
- Cloud
- Python SDK
- CeasedOperations
---

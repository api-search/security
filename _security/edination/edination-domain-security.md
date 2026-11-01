---
api_specs:
- filename: edination-openapi-generated.yml
  format: yaml
  label: EdiNation API
  slug: edination-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edination/openapi/_ae-authored/edination-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edination.com
  spf: true
hosts:
- cert_expires: Jan 11 18:33:52 2027 GMT
  host: edination.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Edination Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EdiNation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EdiNation
provider_slug: edination
slug: edination-domain-security
source_filename: edination-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edination.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 18:33:52 2027 GMT\n  hsts: false\ndomains:\n- domain: edination.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/edination/security/edination-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- EDI
- Healthcare
- Validation
- Open Source
---

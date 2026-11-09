---
api_specs:
- filename: ecocitizenz-com-openapi-generated.yml
  format: yaml
  label: EcoCitizenz API
  slug: ecocitizenz-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocitizenz-com/openapi/_ae-authored/ecocitizenz-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecocitizenz.com
  spf: true
hosts:
- cert_expires: Jan 16 11:45:03 2027 GMT
  host: ecocitizenz.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ecocitizenz Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EcoCitizenz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EcoCitizenz
provider_slug: ecocitizenz-com
slug: ecocitizenz-com-domain-security
source_filename: ecocitizenz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecocitizenz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:45:03 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: ecocitizenz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ecocitizenz-com/security/ecocitizenz-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Trust
- Security
- Platform
- Enterprise
---

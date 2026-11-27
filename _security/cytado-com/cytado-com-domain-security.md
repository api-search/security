---
api_specs:
- filename: cytado-com-openapi-generated.yml
  format: yaml
  label: Cytado API
  slug: cytado-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cytado-com/openapi/_ae-authored/cytado-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cytado.com
  spf: true
hosts:
- cert_expires: Jan 19 09:00:30 2027 GMT
  host: cytado.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cytado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cytado, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cytado
provider_slug: cytado-com
slug: cytado-com-domain-security
source_filename: cytado-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cytado.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 09:00:30 2027 GMT\n  hsts: false\ndomains:\n- domain: cytado.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cytado-com/security/cytado-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Citations
- Bibliography
- Academic
- Research
---

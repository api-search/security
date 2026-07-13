---
api_specs:
- filename: hashicorp-nomad-openapi.yml
  format: yaml
  label: HashiCorp Nomad
  slug: hashicorp-nomad
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/openapi/hashicorp-nomad-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nomadproject.io
  spf: true
hosts:
- cert_expires: Sep 26 12:40:58 2026 GMT
  host: www.nomadproject.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Hashicorp Nomad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HashiCorp Nomad, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HashiCorp Nomad
provider_slug: hashicorp-nomad
slug: hashicorp-nomad-domain-security
source_filename: hashicorp-nomad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nomadproject.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:40:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: nomadproject.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashicorp-nomad/refs/heads/main/security/hashicorp-nomad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Containers
- HashiCorp
- Multi-Cloud
- Orchestration
- Scheduling
- Workloads
---

---
api_specs:
- filename: devzero-openapi-generated.yml
  format: yaml
  label: Devzero API
  slug: devzero-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devzero/openapi/_ae-authored/devzero-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: devzero.io
  spf: true
hosts:
- cert_expires: Jan  7 10:47:20 2027 GMT
  host: www.devzero.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Devzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Devzero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Devzero
provider_slug: devzero
slug: devzero-domain-security
source_filename: devzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.devzero.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:47:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: devzero.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/devzero/security/devzero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Kubernetes
- Cloud Cost
- DevOps
- Artificial Intelligence
---

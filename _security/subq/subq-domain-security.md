---
api_specs:
- filename: subq-openapi-generated.yml
  format: yaml
  label: Subquadratic API
  slug: subq-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subq/openapi/_ae-authored/subq-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: subq.ai
  spf: true
hosts:
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: subq.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Subq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subquadratic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Subquadratic
provider_slug: subq
slug: subq-domain-security
source_filename: subq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: subq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: subq.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/subq/security/subq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Enterprise
- Decision Models
- Long Context
---

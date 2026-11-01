---
api_specs:
- filename: socialhook-openapi-generated.yml
  format: yaml
  label: Lead Lock Systems API
  slug: socialhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialhook/openapi/_ae-authored/socialhook-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: socialhook.io
  spf: true
hosts:
- cert_expires: Dec 18 05:49:07 2026 GMT
  host: socialhook.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Socialhook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lead Lock Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lead Lock Systems
provider_slug: socialhook
slug: socialhook-domain-security
source_filename: socialhook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socialhook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 05:49:07 2026 GMT\n  hsts: false\ndomains:\n- domain: socialhook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/socialhook/security/socialhook-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Webhook
- Social Media
- Integration
- Automation
---

---
api_specs:
- filename: kanbai-app-sops-api-openapi.yml
  format: yaml
  label: Kanbai Sops API
  slug: kanbai-app-sops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanbai-app/openapi/kanbai-app-sops-api-openapi.yml
- filename: kanbai-app-templates-api-openapi.yml
  format: yaml
  label: Kanbai Templates API
  slug: kanbai-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanbai-app/openapi/kanbai-app-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kanbai.app
  spf: false
hosts:
- cert_expires: Jan  9 15:52:08 2027 GMT
  host: kanbai.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kanbai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanbai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Kanbai
provider_slug: kanbai-app
slug: kanbai-app-domain-security
source_filename: kanbai-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kanbai.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 15:52:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kanbai.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kanbai-app/security/kanbai-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Project Management
- Artificial Intelligence
- Collaboration
- Software-as-a-Service
---

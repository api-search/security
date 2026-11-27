---
api_specs:
- filename: partli-app-guides-openapi-generated.yml
  format: yaml
  label: Partli guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/partli-app/openapi/_ae-authored/partli-app-guides-openapi-generated.yml
- filename: partli-app-install-openapi-generated.yml
  format: yaml
  label: Partli install API
  slug: install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/partli-app/openapi/_ae-authored/partli-app-install-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: partli.app
  spf: true
hosts:
- cert_expires: Jan 13 04:25:02 2027 GMT
  host: partli.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Partli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Partli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Partli
provider_slug: partli-app
slug: partli-app-domain-security
source_filename: partli-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partli.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 04:25:02 2027 GMT\n  hsts: false\ndomains:\n- domain: partli.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/partli-app/security/partli-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Affiliates
- Software-as-a-Service
- Artificial Intelligence
- Payments
- Partner Programs
---

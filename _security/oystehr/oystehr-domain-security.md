---
api_specs:
- filename: oystehr-openapi-generated.yml
  format: yaml
  label: Oystehr API
  slug: oystehr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oystehr/openapi/_ae-authored/oystehr-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oystehr.com
  spf: true
hosts:
- cert_expires: Dec 20 05:35:51 2026 GMT
  host: oystehr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oystehr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oystehr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oystehr
provider_slug: oystehr
slug: oystehr-domain-security
source_filename: oystehr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oystehr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 05:35:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oystehr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oystehr/security/oystehr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HealthTech
- EHR
- API
- DeveloperFirst
---

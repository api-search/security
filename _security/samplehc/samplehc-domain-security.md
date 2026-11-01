---
api_specs:
- filename: samplehc-openapi-generated.yml
  format: yaml
  label: Sample API
  slug: samplehc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samplehc/openapi/_ae-authored/samplehc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: samplehc.com
  spf: true
hosts:
- cert_expires: Jan 16 11:36:32 2027 GMT
  host: samplehc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Samplehc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sample, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sample
provider_slug: samplehc
slug: samplehc-domain-security
source_filename: samplehc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: samplehc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:36:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: samplehc.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/samplehc/security/samplehc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Artificial Intelligence
- Document Automation
- LLM
- Software-as-a-Service
---

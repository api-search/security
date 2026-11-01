---
api_specs:
- filename: latchbio-openapi-generated.yml
  format: yaml
  label: LatchBio API
  slug: latchbio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latchbio/openapi/_ae-authored/latchbio-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: latch.bio
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: latch.bio
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latchbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LatchBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LatchBio
provider_slug: latchbio
slug: latchbio-domain-security
source_filename: latchbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latch.bio\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: latch.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/latchbio/security/latchbio-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Biotechnology
- LabAutomation
- DataAnalytics
- MachineLearning
- Platform
- Company
---

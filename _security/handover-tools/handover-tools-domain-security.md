---
api_specs:
- filename: handover-tools-openapi-generated.yml
  format: yaml
  label: Handover Tools API
  slug: handover-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-tools/openapi/_ae-authored/handover-tools-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: handover.tools
  spf: true
hosts:
- cert_expires: Jan  7 01:18:36 2027 GMT
  host: handover.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Handover Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handover Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Handover Tools
provider_slug: handover-tools
slug: handover-tools-domain-security
source_filename: handover-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handover.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 01:18:36 2027 GMT\n  hsts: false\ndomains:\n- domain: handover.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/handover-tools/security/handover-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Encryption
- Communications
- Tools
- Security
---

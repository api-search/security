---
api_specs:
- filename: refold-openapi-generated.yml
  format: yaml
  label: Refold API
  slug: refold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/refold/openapi/_ae-authored/refold-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: refold.ai
  spf: true
hosts:
- cert_expires: Nov 30 06:40:31 2026 GMT
  host: www.refold.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Refold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Refold
provider_slug: refold
slug: refold-domain-security
source_filename: refold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.refold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 06:40:31 2026 GMT\n  hsts: false\ndomains:\n- domain: refold.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/refold/security/refold-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Integration
- Enterprise
- Automation
---

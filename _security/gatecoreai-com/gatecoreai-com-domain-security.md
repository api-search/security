---
api_specs:
- filename: gatecoreai-com-openapi-generated.yml
  format: yaml
  label: GateCore AI API
  slug: gatecoreai-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatecoreai-com/openapi/_ae-authored/gatecoreai-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gatecoreai.com
  spf: true
hosts:
- cert_expires: Jan 11 07:28:34 2027 GMT
  host: gatecoreai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GateCore AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GateCore AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GateCore AI
provider_slug: gatecoreai-com
slug: gatecoreai-com-domain-security
source_filename: gatecoreai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gatecoreai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 07:28:34 2027 GMT\n  hsts: false\ndomains:\n- domain: gatecoreai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gatecoreai-com/security/gatecoreai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Platform
- Governance
- Marketplace
- Security
- Enterprise
---

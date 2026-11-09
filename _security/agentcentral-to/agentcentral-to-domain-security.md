---
api_specs:
- filename: agentcentral-to-openapi-generated.yml
  format: yaml
  label: Agent Central API
  slug: agentcentral-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcentral-to/openapi/_ae-authored/agentcentral-to-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentcentral.to
  spf: true
hosts:
- cert_expires: Dec 22 08:26:21 2026 GMT
  host: agentcentral.to
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentcentral To Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Central, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agent Central
provider_slug: agentcentral-to
slug: agentcentral-to-domain-security
source_filename: agentcentral-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentcentral.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 08:26:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentcentral.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentcentral-to/security/agentcentral-to-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Artificial Intelligence
- Automation
- Amazon
- Seller Central
---

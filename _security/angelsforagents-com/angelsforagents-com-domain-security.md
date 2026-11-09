---
api_specs:
- filename: openapi.json
  format: json
  label: Angels for Agents Discovery API
  slug: angels-for-agents-discovery-api
  spec_type: OpenAPI
  url: https://angelsforagents.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: angelsforagents.com
  spf: true
hosts:
- cert_expires: Dec 24 16:40:35 2026 GMT
  host: angelsforagents.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Angelsforagents Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angels for Agents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Angels for Agents
provider_slug: angelsforagents-com
slug: angelsforagents-com-domain-security
source_filename: angelsforagents-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: angelsforagents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 16:40:35 2026 GMT\n  hsts: false\ndomains:\n- domain: angelsforagents.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/angelsforagents-com/security/angelsforagents-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Capital
- Artificial Intelligence
- Agents
- Venture Funding
- Networks
---

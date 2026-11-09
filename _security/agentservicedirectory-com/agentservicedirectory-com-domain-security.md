---
api_specs:
- filename: openapi.json
  format: json
  label: Agent Service Directory API
  slug: agent-service-directory-api
  spec_type: OpenAPI
  url: https://agentservicedirectory.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentservicedirectory.com
  spf: true
hosts:
- cert_expires: Jan 15 07:32:09 2027 GMT
  host: agentservicedirectory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentservicedirectory Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Service Directory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agent Service Directory
provider_slug: agentservicedirectory-com
slug: agentservicedirectory-com-domain-security
source_filename: agentservicedirectory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentservicedirectory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 07:32:09 2027 GMT\n  hsts: false\ndomains:\n- domain: agentservicedirectory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentservicedirectory-com/security/agentservicedirectory-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Agents
- Directory
- Marketplace
- Metrics
---

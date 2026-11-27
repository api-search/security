---
api_specs:
- filename: agent-tune-com-openapi-generated.yml
  format: yaml
  label: AgentTune API
  slug: agent-tune-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-tune-com/openapi/_ae-authored/agent-tune-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agent-tune.com
  spf: true
hosts:
- cert_expires: Dec 20 12:09:47 2026 GMT
  host: agent-tune.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentTune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentTune, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgentTune
provider_slug: agent-tune-com
slug: agent-tune-com-domain-security
source_filename: agent-tune-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-tune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 12:09:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agent-tune.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agent-tune-com/security/agent-tune-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---

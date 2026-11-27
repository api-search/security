---
api_specs:
- filename: agent-manifest-com-openapi-generated.yml
  format: yaml
  label: Agent Manifest API
  slug: agent-manifest-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manifest-com/openapi/_ae-authored/agent-manifest-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agent-manifest.com
  spf: true
hosts:
- cert_expires: Jan  8 05:06:02 2027 GMT
  host: agent-manifest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Manifest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Manifest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agent Manifest
provider_slug: agent-manifest-com
slug: agent-manifest-com-domain-security
source_filename: agent-manifest-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-manifest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 05:06:02 2027 GMT\n  hsts: false\ndomains:\n- domain: agent-manifest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agent-manifest-com/security/agent-manifest-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Protocol
- Registry
- Validation
- Open Source
---

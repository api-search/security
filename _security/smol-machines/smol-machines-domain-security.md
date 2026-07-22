---
api_specs:
- filename: smol-machines-smolfleet-openapi.json
  format: json
  label: Smol Machines Cloud API (smolfleet)
  slug: smol-machines-cloud-api-smolfleet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-smolfleet-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smolmachines.com
  spf: true
hosts:
- cert_expires: Sep 11 13:03:12 2026 GMT
  host: smolmachines.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 02:29:30 2026 GMT
  host: api.smolmachines.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smol Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smol Machines, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smol Machines
provider_slug: smol-machines
slug: smol-machines-domain-security
source_filename: smol-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smolmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:03:12 2026 GMT\n  hsts: false\n- host: api.smolmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 02:29:30 2026 GMT\n  hsts: null\ndomains:\n- domain: smolmachines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/security/smol-machines-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- MicroVM
- Sandbox
- Virtualization
- Developer Tools
- Infrastructure
- AI Agents
- Code Execution
- Containers
- Cloud
---

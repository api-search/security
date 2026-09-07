---
api_specs:
- filename: volumez-orchestrator-api-openapi.yaml
  format: yaml
  label: Volumez Orchestrator API
  slug: volumez-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumez/refs/heads/main/openapi/volumez-orchestrator-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: volumez.com
  spf: true
hosts:
- cert_expires: Nov  6 18:16:19 2026 GMT
  host: volumez.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.dev.volumez.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Volumez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volumez, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Volumez
provider_slug: volumez
slug: volumez-domain-security
source_filename: volumez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volumez.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 18:16:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dev.volumez.com\n  https: false\ndomains:\n- domain: volumez.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volumez/refs/heads/main/security/volumez-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Storage
- Block Storage
- Data Infrastructure
- Cloud Infrastructure
- Kubernetes
- Container Storage Interface
- AI Infrastructure
- Snapshots
- Infrastructure as Code
- DIaaS
---

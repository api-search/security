---
api_specs:
- filename: artifact-hub-openapi.yml
  format: yaml
  label: Artifact Hub API
  slug: artifact-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/openapi/artifact-hub-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artifacthub.io
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: artifacthub.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artifact Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artifact Hub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artifact Hub
provider_slug: artifact-hub
slug: artifact-hub-domain-security
source_filename: artifact-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artifacthub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: artifacthub.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifact-hub/refs/heads/main/security/artifact-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- CNCF
- Helm Charts
- Package Registry
- Discovery
- Open Source
---

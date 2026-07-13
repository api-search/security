---
api_specs:
- filename: packer-openapi.yml
  format: yaml
  label: Packer
  slug: packer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packer/refs/heads/main/openapi/packer-openapi.yml
- filename: packer-openapi.yml
  format: yaml
  label: HCP Packer Artifact Registry API
  slug: hcp-packer-artifact-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packer/refs/heads/main/openapi/packer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: packer.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashicorp.com
  spf: true
hosts:
- cert_expires: Aug 26 18:49:45 2026 GMT
  host: www.packer.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:45:45 2026 GMT
  host: developer.hashicorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.cloud.hashicorp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Packer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Packer
provider_slug: packer
slug: packer-domain-security
source_filename: packer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.packer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cloud.hashicorp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: packer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packer/refs/heads/main/security/packer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- DevOps
- HashiCorp
- Image Building
- Infrastructure as Code
---

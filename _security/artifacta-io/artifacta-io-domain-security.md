---
api_specs:
- filename: artifacta-io-openapi.json
  format: json
  label: Artifacta API
  slug: artifacta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artifacta-io/openapi/artifacta-io-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: artifacta.io
  spf: true
hosts:
- cert_expires: Dec 30 16:14:08 2026 GMT
  host: artifacta.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artifacta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artifacta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Artifacta
provider_slug: artifacta-io
slug: artifacta-io-domain-security
source_filename: artifacta-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artifacta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 16:14:08 2026 GMT\n  hsts: null\ndomains:\n- domain: artifacta.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/artifacta-io/security/artifacta-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Storage
- Artifact
- MCP
- Open Source
---

---
api_specs:
- filename: blocksigner-org-agent-world-12-api-openapi.yml
  format: yaml
  label: BlockSigner Agent World (12) API
  slug: blocksigner-org-agent-world-12-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blocksigner-org/openapi/blocksigner-org-agent-world-12-api-openapi.yml
- filename: blocksigner-org-free-api-openapi.yml
  format: yaml
  label: BlockSigner Free API
  slug: blocksigner-org-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blocksigner-org/openapi/blocksigner-org-free-api-openapi.yml
- filename: blocksigner-org-provenance-5-api-openapi.yml
  format: yaml
  label: BlockSigner Provenance (5) API
  slug: blocksigner-org-provenance-5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blocksigner-org/openapi/blocksigner-org-provenance-5-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blocksigner.org
  spf: true
hosts:
- cert_expires: Jan 14 01:09:25 2027 GMT
  host: blocksigner.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blocksigner Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockSigner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BlockSigner
provider_slug: blocksigner-org
slug: blocksigner-org-domain-security
source_filename: blocksigner-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blocksigner.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 01:09:25 2027 GMT\n  hsts: null\ndomains:\n- domain: blocksigner.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/blocksigner-org/security/blocksigner-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

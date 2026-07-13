---
api_specs:
- filename: openapi-typescript-codegen
  format: yaml
  label: Dotmatics Luma API
  slug: dotmatics-luma-api
  spec_type: OpenAPI
  url: https://github.com/dotmatics/openapi-typescript-codegen
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dotmatics.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.dotmatics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.dotmatics.com
  https: false
kind: domain-security
layout: security
method: probed
name: Dotmatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dotmatics, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dotmatics
provider_slug: dotmatics
slug: dotmatics-domain-security
source_filename: dotmatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dotmatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dotmatics.com\n  https: false\ndomains:\n- domain: dotmatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotmatics/refs/heads/main/security/dotmatics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scientific Informatics
- Pharma
- Biotech
- Drug Discovery
- ELN
- LIMS
- Compound Registration
- Experimental Data
- R&D
---

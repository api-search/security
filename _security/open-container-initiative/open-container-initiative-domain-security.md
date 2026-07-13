---
api_specs:
- filename: open-container-initiative-openapi.yml
  format: yaml
  label: Open Container Initiative
  slug: open-container-initiative
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-container-initiative/refs/heads/main/openapi/open-container-initiative-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencontainers.org
  spf: false
hosts:
- cert_expires: Sep 25 06:21:26 2026 GMT
  host: opencontainers.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Container Initiative Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Container Initiative, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Container Initiative
provider_slug: open-container-initiative
slug: open-container-initiative-domain-security
source_filename: open-container-initiative-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencontainers.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:21:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opencontainers.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-container-initiative/refs/heads/main/security/open-container-initiative-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Containers
- OCI
- Open Source
- Standards
---

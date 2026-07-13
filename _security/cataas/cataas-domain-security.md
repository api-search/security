---
api_specs:
- filename: cataas-openapi-original.yml
  format: yaml
  label: Cataas
  slug: cataas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/openapi/cataas-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cataas.com
  spf: true
hosts:
- cert_expires: Sep 19 08:40:52 2026 GMT
  host: cataas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cataas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cataas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cataas
provider_slug: cataas
slug: cataas-domain-security
source_filename: cataas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cataas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:40:52 2026 GMT\n  hsts: null\ndomains:\n- domain: cataas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/security/cataas-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Animals
- Cats
- Images
- Open Source
- Public APIs
---

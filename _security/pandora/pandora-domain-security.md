---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Pandora GraphQL API
  slug: pandora-graphql-api
  spec_type: OpenAPI
  url: https://developer.pandora.com/docs/reference/graphql/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pandora.com
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: developer.pandora.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: ce.pandora.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pandora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pandora, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pandora
provider_slug: pandora
slug: pandora-domain-security
source_filename: pandora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.pandora.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\n- host: ce.pandora.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pandora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandora/refs/heads/main/security/pandora-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Music
- Streaming
- Radio
- Podcasts
- Music Genome Project
- Personalization
---

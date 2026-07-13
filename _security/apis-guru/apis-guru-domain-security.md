---
api_specs:
- filename: apis-guru-openapi.yaml
  format: yaml
  label: APIs.guru REST API
  slug: apis-guru-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/openapi/apis-guru-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apis.guru
  spf: true
hosts:
- cert_expires: Sep 15 15:09:58 2026 GMT
  host: apis.guru
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 02:24:31 2026 GMT
  host: api.apis.guru
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apis Guru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIs.guru, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APIs.guru
provider_slug: apis-guru
slug: apis-guru-domain-security
source_filename: apis-guru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apis.guru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:09:58 2026 GMT\n  hsts: false\n- host: api.apis.guru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 02:24:31 2026 GMT\n  hsts: null\ndomains:\n- domain: apis.guru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/security/apis-guru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Catalog
- API Directory
- API Discovery
- Community
- GraphQL
- Open Source
- OpenAPI
---

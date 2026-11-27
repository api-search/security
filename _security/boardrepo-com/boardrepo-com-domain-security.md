---
api_specs:
- filename: boardrepo-com-openapi-generated.yml
  format: yaml
  label: BoardRepo API
  slug: boardrepo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardrepo-com/openapi/_ae-authored/boardrepo-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: boardrepo.com
  spf: true
hosts:
- cert_expires: Jan 29 12:34:17 2027 GMT
  host: boardrepo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BoardRepo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoardRepo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BoardRepo
provider_slug: boardrepo-com
slug: boardrepo-com-domain-security
source_filename: boardrepo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boardrepo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 12:34:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: boardrepo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/boardrepo-com/security/boardrepo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Hardware
- KiCad
- Collaboration
- Open Source
- Design
---

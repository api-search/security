---
api_specs:
- filename: remem-me-access-api-openapi.yml
  format: yaml
  label: remem-me Access API
  slug: remem-me-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/remem-me/openapi/remem-me-access-api-openapi.yml
- filename: remem-me-collections-api-openapi.yml
  format: yaml
  label: remem-me Collections API
  slug: remem-me-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/remem-me/openapi/remem-me-collections-api-openapi.yml
- filename: remem-me-replication-api-openapi.yml
  format: yaml
  label: remem-me Replication API
  slug: remem-me-replication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/remem-me/openapi/remem-me-replication-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: remem.me
  spf: true
hosts:
- cert_expires: Jan 25 08:00:47 2027 GMT
  host: remem.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Remem Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for remem-me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: remem-me
provider_slug: remem-me
slug: remem-me-domain-security
source_filename: remem-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remem.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 08:00:47 2027 GMT\n  hsts: false\ndomains:\n- domain: remem.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/remem-me/security/remem-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Bible
- Memory
- Nonprofit
- Education
- MobileApp
- OpenSource
---

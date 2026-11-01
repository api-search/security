---
api_specs:
- filename: serpkite-com-openapi-generated.yml
  format: yaml
  label: serpkite-com API
  slug: serpkite-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpkite-com/openapi/_ae-authored/serpkite-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: serpkite.com
  spf: true
hosts:
- cert_expires: Dec 31 11:23:45 2026 GMT
  host: serpkite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Serpkite Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for serpkite-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: serpkite-com
provider_slug: serpkite-com
slug: serpkite-com-domain-security
source_filename: serpkite-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serpkite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 11:23:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: serpkite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/serpkite-com/security/serpkite-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Search
- Data Retrieval
- API
- Developer Platform
---

---
api_specs:
- filename: citefiles-com-openapi-generated.yml
  format: yaml
  label: Cite Files API
  slug: citefiles-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citefiles-com/openapi/_ae-authored/citefiles-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: citefiles.com
  spf: true
hosts:
- cert_expires: Jan 16 13:30:21 2027 GMT
  host: citefiles.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cite Files Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cite Files, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cite Files
provider_slug: citefiles-com
slug: citefiles-com-domain-security
source_filename: citefiles-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citefiles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 13:30:21 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: citefiles.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/citefiles-com/security/citefiles-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Crawling
- Accessibility
- Open Source
---

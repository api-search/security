---
api_specs:
- filename: refetch-cloud-openapi-generated.yml
  format: yaml
  label: Refetch API
  slug: refetch-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/refetch-cloud/openapi/_ae-authored/refetch-cloud-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: refetch.cloud
  spf: true
hosts:
- cert_expires: Feb  3 12:12:44 2027 GMT
  host: refetch.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Refetch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refetch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Refetch
provider_slug: refetch-cloud
slug: refetch-cloud-domain-security
source_filename: refetch-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: refetch.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 12:12:44 2027 GMT\n  hsts: false\ndomains:\n- domain: refetch.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/refetch-cloud/security/refetch-cloud-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- WebFetching
- Automation
- DataExtraction
---

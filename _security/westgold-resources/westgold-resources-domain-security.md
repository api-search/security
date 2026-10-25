---
api_specs:
- filename: westgold-resources-openapi-generated.yml
  format: yaml
  label: Westgold Resources API
  slug: westgold-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/westgold-resources/refs/heads/main/openapi/_ae-authored/westgold-resources-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: westgold.com.au
  spf: true
hosts:
- cert_expires: Dec 15 02:33:46 2026 GMT
  host: www.westgold.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Westgold Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Westgold Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Westgold Resources
provider_slug: westgold-resources
slug: westgold-resources-domain-security
source_filename: westgold-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westgold.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 02:33:46 2026 GMT\n  hsts: null\ndomains:\n- domain: westgold.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westgold-resources/refs/heads/main/security/westgold-resources-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gold
- Mining
- Australia
- ASX
- Natural Resources
---

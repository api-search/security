---
api_specs:
- filename: catchdoms-domains-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Domains API
  slug: catchdoms-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-domains-api-openapi.yml
- filename: catchdoms-free-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Free API
  slug: catchdoms-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-free-api-openapi.yml
- filename: catchdoms-pending-delete-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Pending Delete API
  slug: catchdoms-pending-delete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-pending-delete-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: catchdoms.com
  spf: true
hosts:
- cert_expires: Dec  7 17:29:47 2026 GMT
  host: catchdoms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Catchdoms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CatchDoms Expired Domains API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CatchDoms Expired Domains API
provider_slug: catchdoms
slug: catchdoms-domain-security
source_filename: catchdoms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catchdoms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 17:29:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: catchdoms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/security/catchdoms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Domains
- SEO
- Expired
---

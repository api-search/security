---
api_specs:
- filename: aspiresingapore-openapi-generated.yml
  format: yaml
  label: Aspiresingapore API
  slug: aspiresingapore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspiresingapore/refs/heads/main/openapi/_ae-authored/aspiresingapore-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aspireapp.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: aspireapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aspiresingapore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aspiresingapore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aspiresingapore
provider_slug: aspiresingapore
slug: aspiresingapore-domain-security
source_filename: aspiresingapore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aspireapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aspireapp.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspiresingapore/refs/heads/main/security/aspiresingapore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Banking
- API
- Singapore
- SaaS
---

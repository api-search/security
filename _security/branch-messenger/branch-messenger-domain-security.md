---
api_specs:
- filename: branch-messenger-openapi-generated.yml
  format: yaml
  label: Branch API
  slug: branch-messenger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/branch-messenger/refs/heads/main/openapi/_ae-authored/branch-messenger-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: branch.io
  spf: true
hosts:
- cert_expires: Nov 19 08:22:26 2026 GMT
  host: www.branch.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Branch Messenger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Branch
provider_slug: branch-messenger
slug: branch-messenger-domain-security
source_filename: branch-messenger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.branch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 08:22:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: branch.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branch-messenger/refs/heads/main/security/branch-messenger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile
- DeepLinking
- Attribution
- Marketing
- Analytics
---

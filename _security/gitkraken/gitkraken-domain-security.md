---
api_specs:
- filename: gitkraken-openapi-generated.yml
  format: yaml
  label: GitKraken API
  slug: gitkraken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitkraken/refs/heads/main/openapi/_ae-authored/gitkraken-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitkraken.com
  spf: true
hosts:
- cert_expires: Nov 16 20:27:53 2026 GMT
  host: www.gitkraken.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gitkraken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitKraken, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GitKraken
provider_slug: gitkraken
slug: gitkraken-domain-security
source_filename: gitkraken-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gitkraken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 20:27:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: gitkraken.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitkraken/refs/heads/main/security/gitkraken-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Git
- Artificial Intelligence
- Collaboration
- Platform
---

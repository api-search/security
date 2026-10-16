---
api_specs:
- filename: algorithmia-openapi-generated.yml
  format: yaml
  label: Algorithmia API
  slug: algorithmia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algorithmia/refs/heads/main/openapi/_ae-authored/algorithmia-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datarobot.com
  spf: true
hosts:
- cert_expires: Dec 25 12:09:31 2026 GMT
  host: www.datarobot.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Algorithmia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Algorithmia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Algorithmia
provider_slug: algorithmia
slug: algorithmia-domain-security
source_filename: algorithmia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datarobot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 12:09:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: datarobot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algorithmia/refs/heads/main/security/algorithmia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Machine-Learning
- Marketplace
- Platform
- DataRobot
---

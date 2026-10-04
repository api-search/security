---
api_specs:
- filename: tabnine-openapi-generated.yml
  format: yaml
  label: Tabnine API
  slug: tabnine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabnine/refs/heads/main/openapi/_ae-authored/tabnine-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tabnine.com
  spf: true
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: www.tabnine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tabnine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabnine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tabnine
provider_slug: tabnine
slug: tabnine-domain-security
source_filename: tabnine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tabnine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tabnine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabnine/refs/heads/main/security/tabnine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Developer Tools
- Code Completion
- Self-Hosted
- Enterprise
- Privacy
---

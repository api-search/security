---
api_specs:
- filename: alium-openapi-generated.yml
  format: yaml
  label: Alium API
  slug: alium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alium/refs/heads/main/openapi/_ae-authored/alium-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alium.io
  spf: true
hosts:
- cert_expires: Dec 24 06:22:31 2026 GMT
  host: www.alium.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alium
provider_slug: alium
slug: alium-domain-security
source_filename: alium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 06:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: alium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alium/refs/heads/main/security/alium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vendor research
- Marketing intelligence
- E‑commerce
- Enterprise tech
---

---
api_specs:
- filename: bind-openapi-generated.yml
  format: yaml
  label: Bind API
  slug: bind-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bind/refs/heads/main/openapi/_ae-authored/bind-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bindhq.com
  spf: true
hosts:
- cert_expires: Dec 20 06:08:35 2026 GMT
  host: www.bindhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bind
provider_slug: bind
slug: bind-domain-security
source_filename: bind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bindhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 06:08:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bindhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bind/refs/heads/main/security/bind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Platform
- API
- Composable
- Specialty
---

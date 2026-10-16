---
api_specs:
- filename: ciq-openapi-generated.yml
  format: yaml
  label: CIQ API
  slug: ciq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/_ae-authored/ciq-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ciq.com
  spf: true
hosts:
- cert_expires: Nov 26 08:14:00 2026 GMT
  host: ciq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ciq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CIQ
provider_slug: ciq
slug: ciq-domain-security
source_filename: ciq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ciq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 08:14:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ciq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/security/ciq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Infrastructure
- Open-Source
- Enterprise
- Cloud
---

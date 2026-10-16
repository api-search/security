---
api_specs:
- filename: nice-openapi-generated.yml
  format: yaml
  label: NICE API
  slug: nice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/openapi/_ae-authored/nice-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nice.com
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: www.nice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NICE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NICE
provider_slug: nice
slug: nice-domain-security
source_filename: nice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nice/refs/heads/main/security/nice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- CustomerExperience
- AI
- Cloud
- Integration
---

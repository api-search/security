---
api_specs:
- filename: quietstance-inquiries-api-openapi.yml
  format: yaml
  label: Quiet Stance Inquiries API
  slug: quietstance-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietstance/refs/heads/main/openapi/quietstance-inquiries-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quietstance.com
  spf: true
hosts:
- cert_expires: Dec  6 18:17:03 2026 GMT
  host: quietstance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quietstance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quiet Stance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quiet Stance
provider_slug: quietstance
slug: quietstance-domain-security
source_filename: quietstance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quietstance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 18:17:03 2026 GMT\n  hsts: false\ndomains:\n- domain: quietstance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quietstance/refs/heads/main/security/quietstance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure
- Project Development
- Collaboration
---

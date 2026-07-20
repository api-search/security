---
api_specs:
- filename: brainbase-openapi-original.json
  format: json
  label: Brainbase API v1
  slug: brainbase-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainbase/refs/heads/main/openapi/brainbase-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brainbase.com
  spf: true
hosts:
- host: www.brainbase.com
  https: false
- cert_expires: Sep 18 21:02:55 2026 GMT
  host: api.brainbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brainbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brainbase, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brainbase
provider_slug: brainbase
slug: brainbase-domain-security
source_filename: brainbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brainbase.com\n  https: false\n- host: api.brainbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:02:55 2026 GMT\n  hsts: null\ndomains:\n- domain: brainbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainbase/refs/heads/main/security/brainbase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Intellectual Property
- Brand Licensing
- Licensing Management
- Royalties
- Contracts
- Trademarks
- SaaS
---

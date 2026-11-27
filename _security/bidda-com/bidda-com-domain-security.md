---
api_specs:
- filename: bidda-com-openapi-generated.yml
  format: yaml
  label: Bidda API
  slug: bidda-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidda-com/openapi/_ae-authored/bidda-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bidda.com
  spf: true
hosts:
- cert_expires: Dec 29 14:03:39 2026 GMT
  host: bidda.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bidda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bidda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bidda
provider_slug: bidda-com
slug: bidda-com-domain-security
source_filename: bidda-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 14:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bidda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bidda-com/security/bidda-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- Regulations
- Artificial Intelligence
- Data
---

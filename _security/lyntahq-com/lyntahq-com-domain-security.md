---
api_specs:
- filename: lyntahq-com-ask-api-openapi.yml
  format: yaml
  label: Lynta Ask API
  slug: lyntahq-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lyntahq-com/openapi/lyntahq-com-ask-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lyntahq.com
  spf: true
hosts:
- cert_expires: Jan  3 22:30:47 2027 GMT
  host: lyntahq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lynta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lynta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lynta
provider_slug: lyntahq-com
slug: lyntahq-com-domain-security
source_filename: lyntahq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lyntahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 22:30:47 2027 GMT\n  hsts: false\ndomains:\n- domain: lyntahq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lyntahq-com/security/lyntahq-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Real-Time
- Infrastructure
- Artificial Intelligence
- Collaboration
- Developers
---

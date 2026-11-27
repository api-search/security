---
api_specs:
- filename: liner-com-openapi-generated.yml
  format: yaml
  label: Liner API
  slug: liner-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liner-com/openapi/_ae-authored/liner-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: liner.com
  spf: true
hosts:
- cert_expires: Feb  2 10:49:13 2027 GMT
  host: liner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Liner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Liner
provider_slug: liner-com
slug: liner-com-domain-security
source_filename: liner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 10:49:13 2027 GMT\n  hsts: false\ndomains:\n- domain: liner.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/liner-com/security/liner-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Research
- Agents
- Platform
- Productivity
---

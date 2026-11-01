---
api_specs:
- filename: digibee-com-digibee-api-api-openapi.yml
  format: yaml
  label: Digibee API
  slug: digibee-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digibee-com/openapi/digibee-com-digibee-api-api-openapi.yml
- filename: digibee-com-openapi-generated.yml
  format: yaml
  label: Digibee API
  slug: digibee-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digibee-com/openapi/_ae-authored/digibee-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: digibee.com
  spf: true
hosts:
- cert_expires: Jan 15 00:08:23 2027 GMT
  host: digibee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digibee Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digibee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Digibee
provider_slug: digibee-com
slug: digibee-com-domain-security
source_filename: digibee-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digibee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 00:08:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: digibee.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/digibee-com/security/digibee-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Integration
- Artificial Intelligence
- Automation
- Enterprise
---

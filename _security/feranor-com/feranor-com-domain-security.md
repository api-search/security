---
api_specs:
- filename: feranor-com-administration-api-openapi.yml
  format: yaml
  label: Feranor Administration API
  slug: feranor-com-administration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-administration-api-openapi.yml
- filename: feranor-com-health-api-openapi.yml
  format: yaml
  label: Feranor Health API
  slug: feranor-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-health-api-openapi.yml
- filename: feranor-com-keys-api-openapi.yml
  format: yaml
  label: Feranor Keys API
  slug: feranor-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-keys-api-openapi.yml
- filename: feranor-com-operations-api-openapi.yml
  format: yaml
  label: Feranor Operations API
  slug: feranor-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-operations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: feranor.com
  spf: true
hosts:
- cert_expires: Apr 18 23:59:59 2027 GMT
  host: feranor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Feranor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feranor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Feranor
provider_slug: feranor-com
slug: feranor-com-domain-security
source_filename: feranor-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feranor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: feranor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/feranor-com/security/feranor-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Encryption
- Post-Quantum
- Consulting
- Artificial Intelligence
---

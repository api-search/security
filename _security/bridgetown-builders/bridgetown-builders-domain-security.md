---
api_specs:
- filename: bridgetown-builders-core-openapi-generated.yml
  format: yaml
  label: Bridge Town core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgetown-builders/openapi/_ae-authored/bridgetown-builders-core-openapi-generated.yml
- filename: bridgetown-builders-getting-started-openapi-generated.yml
  format: yaml
  label: Bridge Town getting started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgetown-builders/openapi/_ae-authored/bridgetown-builders-getting-started-openapi-generated.yml
- filename: bridgetown-builders-guides-openapi-generated.yml
  format: yaml
  label: Bridge Town guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgetown-builders/openapi/_ae-authored/bridgetown-builders-guides-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: bridgetown.builders
  spf: false
hosts:
- cert_expires: Dec 25 09:51:00 2026 GMT
  host: bridgetown.builders
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bridge Town Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridge Town, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bridge Town
provider_slug: bridgetown-builders
slug: bridgetown-builders-domain-security
source_filename: bridgetown-builders-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridgetown.builders\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 09:51:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bridgetown.builders\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bridgetown-builders/security/bridgetown-builders-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Artificial Intelligence
- FP&A
- Collaboration
- Version Control
- Company
---

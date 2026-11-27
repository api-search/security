---
api_specs:
- filename: farpy-com-api-keys-api-openapi.yml
  format: yaml
  label: Farpy Api Keys API
  slug: farpy-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-api-keys-api-openapi.yml
- filename: farpy-com-capabilities-api-openapi.yml
  format: yaml
  label: Farpy Capabilities API
  slug: farpy-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-capabilities-api-openapi.yml
- filename: farpy-com-health-api-openapi.yml
  format: yaml
  label: Farpy Health API
  slug: farpy-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-health-api-openapi.yml
- filename: farpy-com-limits-api-openapi.yml
  format: yaml
  label: Farpy Limits API
  slug: farpy-com-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-limits-api-openapi.yml
- filename: farpy-com-pricing-api-openapi.yml
  format: yaml
  label: Farpy Pricing API
  slug: farpy-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-pricing-api-openapi.yml
- filename: farpy-com-renders-api-openapi.yml
  format: yaml
  label: Farpy Renders API
  slug: farpy-com-renders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-renders-api-openapi.yml
- filename: farpy-com-workspace-api-openapi.yml
  format: yaml
  label: Farpy Workspace API
  slug: farpy-com-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: farpy.com
  spf: true
hosts:
- cert_expires: Jan 12 01:35:20 2027 GMT
  host: farpy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Farpy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farpy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Farpy
provider_slug: farpy-com
slug: farpy-com-domain-security
source_filename: farpy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farpy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 01:35:20 2027 GMT\n  hsts: false\ndomains:\n- domain: farpy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/farpy-com/security/farpy-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- GPU
- Rendering
- Blender
- Cloud
---

---
api_specs:
- filename: outscale-clusters-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Clusters API
  slug: outscale-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-clusters-api-openapi.yml
- filename: outscale-myip-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE My Ip API
  slug: outscale-myip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-myip-api-openapi.yml
- filename: outscale-projects-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Projects API
  slug: outscale-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-projects-api-openapi.yml
- filename: outscale-quotas-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Quotas API
  slug: outscale-quotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-quotas-api-openapi.yml
- filename: outscale-templates-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Templates API
  slug: outscale-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outscale/openapi/outscale-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outscale.com
  spf: true
hosts:
- cert_expires: Dec 30 02:02:45 2026 GMT
  host: outscale.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3DS OUTSCALE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 3DS OUTSCALE
provider_slug: outscale
slug: outscale-domain-security
source_filename: outscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outscale.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 02:02:45 2026 GMT\n  hsts: null\ndomains:\n- domain: outscale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/outscale/security/outscale-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Cloud
- IaaS
- Compute
- Storage
- Networking
---

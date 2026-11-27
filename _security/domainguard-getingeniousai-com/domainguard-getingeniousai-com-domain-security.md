---
api_specs:
- filename: domainguard-getingeniousai-com-actions-api-openapi.yml
  format: yaml
  label: DomainGuard (Ingenious AI) Actions API
  slug: domainguard-getingeniousai-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainguard-getingeniousai-com/openapi/domainguard-getingeniousai-com-actions-api-openapi.yml
- filename: domainguard-getingeniousai-com-events-api-openapi.yml
  format: yaml
  label: DomainGuard (Ingenious AI) Events API
  slug: domainguard-getingeniousai-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainguard-getingeniousai-com/openapi/domainguard-getingeniousai-com-events-api-openapi.yml
- filename: domainguard-getingeniousai-com-health-api-openapi.yml
  format: yaml
  label: DomainGuard (Ingenious AI) Health API
  slug: domainguard-getingeniousai-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainguard-getingeniousai-com/openapi/domainguard-getingeniousai-com-health-api-openapi.yml
- filename: domainguard-getingeniousai-com-scans-api-openapi.yml
  format: yaml
  label: DomainGuard (Ingenious AI) Scans API
  slug: domainguard-getingeniousai-com-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainguard-getingeniousai-com/openapi/domainguard-getingeniousai-com-scans-api-openapi.yml
- filename: domainguard-getingeniousai-com-usage-api-openapi.yml
  format: yaml
  label: DomainGuard (Ingenious AI) Usage API
  slug: domainguard-getingeniousai-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainguard-getingeniousai-com/openapi/domainguard-getingeniousai-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getingeniousai.com
  spf: true
hosts:
- cert_expires: Jan 19 21:56:34 2027 GMT
  host: domainguard.getingeniousai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DomainGuard (Ingenious AI) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DomainGuard (Ingenious AI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DomainGuard (Ingenious AI)
provider_slug: domainguard-getingeniousai-com
slug: domainguard-getingeniousai-com-domain-security
source_filename: domainguard-getingeniousai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domainguard.getingeniousai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 21:56:34 2027 GMT\n  hsts: null\ndomains:\n- domain: getingeniousai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/domainguard-getingeniousai-com/security/domainguard-getingeniousai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Domain Impersonation
- Certificate Transparency
- Typosquat Monitoring
- DNS CAA
- Phishing Defense
- Small Business Security
---

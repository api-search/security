---
api_specs:
- filename: churnlens-site-agent-api-openapi.yml
  format: yaml
  label: ChurnLens Agent API
  slug: churnlens-site-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/churnlens-site/openapi/churnlens-site-agent-api-openapi.yml
- filename: churnlens-site-funnel-api-openapi.yml
  format: yaml
  label: ChurnLens Funnel API
  slug: churnlens-site-funnel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/churnlens-site/openapi/churnlens-site-funnel-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: churnlens.site
  spf: true
hosts:
- cert_expires: Dec  2 22:32:54 2026 GMT
  host: churnlens.site
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Churnlens Site Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChurnLens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChurnLens
provider_slug: churnlens-site
slug: churnlens-site-domain-security
source_filename: churnlens-site-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: churnlens.site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 22:32:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: churnlens.site\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/churnlens-site/security/churnlens-site-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Due Diligence
- Finance
- Subscription
- Analytics
---

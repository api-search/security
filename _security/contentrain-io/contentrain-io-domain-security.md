---
api_specs:
- filename: contentrain-io-openapi-generated.yml
  format: yaml
  label: Contentrain API
  slug: contentrain-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contentrain-io/openapi/_ae-authored/contentrain-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contentrain.io
  spf: true
hosts:
- cert_expires: Dec 30 16:23:47 2026 GMT
  host: contentrain.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contentrain Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contentrain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Contentrain
provider_slug: contentrain-io
slug: contentrain-io-domain-security
source_filename: contentrain-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contentrain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 16:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: contentrain.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/contentrain-io/security/contentrain-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Governance
- Developer Tools
- AI content
- Studio Workflow
- Localization
---

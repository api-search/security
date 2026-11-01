---
api_specs:
- filename: curviate-com-openapi.json
  format: json
  label: Curviate API
  slug: curviate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curviate-com/openapi/curviate-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curviate.com
  spf: true
hosts:
- cert_expires: Dec 26 12:15:53 2026 GMT
  host: curviate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curviate Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for curviate-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: curviate-com
provider_slug: curviate-com
slug: curviate-com-domain-security
source_filename: curviate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curviate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:15:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curviate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/curviate-com/security/curviate-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LinkedIn
- API
- Automation
- Agent
---

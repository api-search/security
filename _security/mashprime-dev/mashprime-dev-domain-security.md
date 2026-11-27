---
api_specs:
- filename: mashprime-dev-discovery-api-openapi.yml
  format: yaml
  label: mashprime-dev Discovery API
  slug: mashprime-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mashprime-dev/openapi/mashprime-dev-discovery-api-openapi.yml
- filename: mashprime-dev-posts-api-openapi.yml
  format: yaml
  label: mashprime-dev Posts API
  slug: mashprime-dev-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mashprime-dev/openapi/mashprime-dev-posts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mashprime.dev
  spf: true
hosts:
- cert_expires: Dec 27 23:03:45 2026 GMT
  host: mashprime.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mashprime-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mashprime-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: mashprime-dev
provider_slug: mashprime-dev
slug: mashprime-dev-domain-security
source_filename: mashprime-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mashprime.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mashprime.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mashprime-dev/security/mashprime-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Agentic Systems
- Community
---

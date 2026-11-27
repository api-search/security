---
api_specs:
- filename: jobbi-org-agent-gigs-api-openapi.yml
  format: yaml
  label: Jobbi Agent gigs API
  slug: jobbi-org-agent-gigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobbi-org/openapi/jobbi-org-agent-gigs-api-openapi.yml
- filename: jobbi-org-human-jobs-api-openapi.yml
  format: yaml
  label: Jobbi Human jobs API
  slug: jobbi-org-human-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobbi-org/openapi/jobbi-org-human-jobs-api-openapi.yml
- filename: jobbi-org-mcp-api-openapi.yml
  format: yaml
  label: Jobbi MCP API
  slug: jobbi-org-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobbi-org/openapi/jobbi-org-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jobbi.org
  spf: true
hosts:
- cert_expires: Dec 25 13:50:17 2026 GMT
  host: jobbi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobbi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobbi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Jobbi
provider_slug: jobbi-org
slug: jobbi-org-domain-security
source_filename: jobbi-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobbi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 13:50:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jobbi.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jobbi-org/security/jobbi-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Job Search
- Artificial Intelligence
- Privacy
- Tech Jobs
---

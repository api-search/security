---
api_specs:
- filename: onssa-org-agent-api-openapi.yml
  format: yaml
  label: Onça Agent API
  slug: onssa-org-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onssa-org/openapi/onssa-org-agent-api-openapi.yml
- filename: onssa-org-ask-api-openapi.yml
  format: yaml
  label: Onça Ask API
  slug: onssa-org-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onssa-org/openapi/onssa-org-ask-api-openapi.yml
- filename: onssa-org-feed-api-openapi.yml
  format: yaml
  label: Onça Feed API
  slug: onssa-org-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onssa-org/openapi/onssa-org-feed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onssa.org
  spf: true
hosts:
- cert_expires: Mar 29 23:59:59 2027 GMT
  host: onssa.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onça Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onça, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Onça
provider_slug: onssa-org
slug: onssa-org-domain-security
source_filename: onssa-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onssa.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: onssa.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/onssa-org/security/onssa-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Software-as-a-Service
- Competitive Intelligence
- Brazil
- B2B
---

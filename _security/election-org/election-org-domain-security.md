---
api_specs:
- filename: election-org-openapi-openapi.json
  format: json
  label: Election.org Public Data API Openapi API
  slug: election-org-public-data-api-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/election-org/refs/heads/main/openapi/_original/election-org-openapi-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: election.org
  spf: true
hosts:
- cert_expires: Dec 20 11:32:00 2026 GMT
  host: election.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Election Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Election.org Public Data API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Election.org Public Data API
provider_slug: election-org
slug: election-org-domain-security
source_filename: election-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: election.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 11:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: election.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/election-org/refs/heads/main/security/election-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Elections
- Public Records
- Data API
- Campaign Finance
- Government
- Political Data
---

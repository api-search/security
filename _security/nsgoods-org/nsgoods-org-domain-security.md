---
api_specs:
- filename: nsgoods-org-health-api-openapi.yml
  format: yaml
  label: nsgoods-org Health API
  slug: nsgoods-org-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nsgoods-org/openapi/nsgoods-org-health-api-openapi.yml
- filename: nsgoods-org-payable-api-openapi.yml
  format: yaml
  label: nsgoods-org Payable API
  slug: nsgoods-org-payable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nsgoods-org/openapi/nsgoods-org-payable-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nsgoods.org
  spf: true
hosts:
- cert_expires: Jan 11 10:53:53 2027 GMT
  host: nsgoods.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nsgoods Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nsgoods-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: nsgoods-org
provider_slug: nsgoods-org
slug: nsgoods-org-domain-security
source_filename: nsgoods-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nsgoods.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 10:53:53 2027 GMT\n  hsts: false\ndomains:\n- domain: nsgoods.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nsgoods-org/security/nsgoods-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Finance
- Blockchain
- Data
- Services
- Company
---

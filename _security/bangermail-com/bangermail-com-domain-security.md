---
api_specs:
- filename: bangermail-com-forms-api-openapi.yml
  format: yaml
  label: BangerMail Inc. Forms API
  slug: bangermail-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bangermail-com/openapi/bangermail-com-forms-api-openapi.yml
- filename: bangermail-com-workspaces-api-openapi.yml
  format: yaml
  label: BangerMail Inc. Workspaces API
  slug: bangermail-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bangermail-com/openapi/bangermail-com-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bangermail.com
  spf: true
hosts:
- cert_expires: Jan 31 04:05:40 2027 GMT
  host: bangermail.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BangerMail Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BangerMail Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BangerMail Inc.
provider_slug: bangermail-com
slug: bangermail-com-domain-security
source_filename: bangermail-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bangermail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 04:05:40 2027 GMT\n  hsts: false\ndomains:\n- domain: bangermail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bangermail-com/security/bangermail-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Artificial Intelligence
- Automation
- Software-as-a-Service
- Marketing
---

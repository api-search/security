---
api_specs:
- filename: formasty-com-capabilities-api-openapi.yml
  format: yaml
  label: Formasty Capabilities API
  slug: formasty-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-capabilities-api-openapi.yml
- filename: formasty-com-forms-api-openapi.yml
  format: yaml
  label: Formasty Forms API
  slug: formasty-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-forms-api-openapi.yml
- filename: formasty-com-me-api-openapi.yml
  format: yaml
  label: Formasty Me API
  slug: formasty-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-me-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: formasty.com
  spf: true
hosts:
- cert_expires: Dec 29 12:44:42 2026 GMT
  host: formasty.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Formasty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formasty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Formasty
provider_slug: formasty-com
slug: formasty-com-domain-security
source_filename: formasty-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formasty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 12:44:42 2026 GMT\n  hsts: false\ndomains:\n- domain: formasty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/formasty-com/security/formasty-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lead Qualification
- Forms
- Artificial Intelligence
- Automation
- Software-as-a-Service
---

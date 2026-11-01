---
api_specs:
- filename: autokitteh-autokitteh-api-api-openapi.yml
  format: yaml
  label: AutoKitteh API
  slug: autokitteh-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autokitteh/openapi/autokitteh-autokitteh-api-api-openapi.yml
- filename: autokitteh-openapi-generated.yml
  format: yaml
  label: AutoKitteh API
  slug: autokitteh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autokitteh/openapi/_ae-authored/autokitteh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: autokitteh.com
  spf: true
hosts:
- cert_expires: Dec 23 00:35:50 2026 GMT
  host: autokitteh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autokitteh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoKitteh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AutoKitteh
provider_slug: autokitteh
slug: autokitteh-domain-security
source_filename: autokitteh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autokitteh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 00:35:50 2026 GMT\n  hsts: false\ndomains:\n- domain: autokitteh.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/autokitteh/security/autokitteh-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Automation
- Orchestration
- Open Source
- Developer Tools
- Workflow Engine
---

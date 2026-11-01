---
api_specs:
- filename: fylamynt-openapi-generated.yml
  format: yaml
  label: Fylamynt API
  slug: fylamynt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fylamynt/openapi/_ae-authored/fylamynt-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fylamynt.com
  spf: true
hosts:
- host: www.fylamynt.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fylamynt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fylamynt, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fylamynt
provider_slug: fylamynt
slug: fylamynt-domain-security
source_filename: fylamynt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fylamynt.com\n  https: false\ndomains:\n- domain: fylamynt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fylamynt/security/fylamynt-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cloud
- Automation
- Incident-Response
- Orchestration
- Platform
---

---
api_specs:
- filename: milestone-openapi-generated.yml
  format: yaml
  label: Milestone API
  slug: milestone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/milestone/openapi/_ae-authored/milestone-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@mstone.ai"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mstone.ai
  spf: true
hosts:
- cert_expires: Jan 12 14:23:13 2027 GMT
  host: www.mstone.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Milestone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Milestone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Milestone
provider_slug: milestone
slug: milestone-domain-security
source_filename: milestone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mstone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 14:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mstone.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@mstone.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/milestone/security/milestone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Spend
- Agent Governance
- AI Productivity
- AI Governance
- KPI Dashboards
---

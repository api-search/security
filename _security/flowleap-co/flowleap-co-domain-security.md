---
api_specs:
- filename: flowleap-co-openapi-generated.yml
  format: yaml
  label: FlowLeap API
  slug: flowleap-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowleap-co/openapi/_ae-authored/flowleap-co-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flowleap.co
  spf: true
hosts:
- cert_expires: Jan 23 06:53:39 2027 GMT
  host: flowleap.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlowLeap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlowLeap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FlowLeap
provider_slug: flowleap-co
slug: flowleap-co-domain-security
source_filename: flowleap-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowleap.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 06:53:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flowleap.co\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flowleap-co/security/flowleap-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Patents
- Artificial Intelligence
- Workspace
- Research
- Drafting
---

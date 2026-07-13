---
api_specs:
- filename: amazon-mechanical-turk-openapi-original.yaml
  format: yaml
  label: Amazon Mechanical Turk API
  slug: amazon-mturk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/openapi/amazon-mechanical-turk-openapi-original.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mturk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: www.mturk.com
  hsts: true
  hsts_max_age: 47474747
  https: true
  tls_version: TLSv1.3
- host: mturk-requester.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Mechanical Turk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Mechanical Turk, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
slug: amazon-mechanical-turk-domain-security
source_filename: amazon-mechanical-turk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mturk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47474747\n- host: mturk-requester.amazonaws.com\n  https: false\ndomains:\n- domain: mturk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/security/amazon-mechanical-turk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
---

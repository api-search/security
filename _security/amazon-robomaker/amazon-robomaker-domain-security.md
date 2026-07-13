---
api_specs:
- filename: amazon-robomaker-openapi.yml
  format: yaml
  label: AWS RoboMaker API
  slug: aws-robomaker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/openapi/amazon-robomaker-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: console.aws.amazon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: robomaker.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Robomaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon RoboMaker, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
slug: amazon-robomaker-domain-security
source_filename: amazon-robomaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: console.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\n- host: robomaker.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/security/amazon-robomaker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Simulation
---

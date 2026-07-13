---
api_specs:
- filename: amazon-app-runner-openapi.yaml
  format: yaml
  label: Amazon App Runner API
  slug: amazon-app-runner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/openapi/amazon-app-runner-openapi.yaml
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
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: console.aws.amazon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: apprunner.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon App Runner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon App Runner, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
slug: amazon-app-runner-domain-security
source_filename: amazon-app-runner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: apprunner.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/security/amazon-app-runner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
---

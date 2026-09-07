---
api_specs:
- filename: continuous-delivery-foundation-jenkins-pipeline-graph-view-openapi.yaml
  format: yaml
  label: Jenkins
  slug: jenkins
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-jenkins-pipeline-graph-view-openapi.yaml
- filename: continuous-delivery-foundation-spinnaker-openapi.json
  format: json
  label: Spinnaker
  slug: spinnaker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-spinnaker-openapi.json
- filename: continuous-delivery-foundation-screwdriver-openapi.json
  format: json
  label: Screwdriver
  slug: screwdriver
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-screwdriver-openapi.json
- filename: continuous-delivery-foundation-jayex-jx-api-openapi.json
  format: json
  label: JayeX
  slug: jayex
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-jayex-jx-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cd.foundation
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cdevents.dev
  spf: false
hosts:
- cert_expires: Oct 26 19:04:59 2026 GMT
  host: cd.foundation
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 04:16:01 2026 GMT
  host: cdevents.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 20:57:55 2026 GMT
  host: www.jenkins.io
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Continuous Delivery Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Continuous Delivery Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Continuous Delivery Foundation
provider_slug: continuous-delivery-foundation
slug: continuous-delivery-foundation-domain-security
source_filename: continuous-delivery-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cd.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 19:04:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: cdevents.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 04:16:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.jenkins.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 18 20:57:55 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: cd.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cdevents.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/security/continuous-delivery-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- CI/CD
- DevOps
- Linux Foundation
- Open-Source
---

---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS Launch Wizard API
  slug: aws-launch-wizard-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/launchwizard/2018-05-10/openapi.yaml
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
- host: launchwizard.amazonaws.com
  https: false
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: launchwizard.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Launch Wizard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Launch Wizard, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Launch Wizard
provider_slug: amazon-launch-wizard
slug: amazon-launch-wizard-domain-security
source_filename: amazon-launch-wizard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: launchwizard.amazonaws.com\n  https: false\n- host: launchwizard.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-launch-wizard/refs/heads/main/security/amazon-launch-wizard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Deployment
- Enterprise Applications
- SAP
- SQL Server
---

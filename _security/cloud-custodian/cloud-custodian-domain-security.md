---
api_specs:
- filename: cloud-custodian-mailer-asyncapi.yml
  format: yaml
  label: Cloud Custodian C7n-Mailer
  slug: cloud-custodian-c7n-mailer
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-custodian/refs/heads/main/asyncapi/cloud-custodian-mailer-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cloudcustodian.io
  spf: false
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: cloudcustodian.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloud Custodian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud Custodian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cloud Custodian
provider_slug: cloud-custodian
slug: cloud-custodian-domain-security
source_filename: cloud-custodian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudcustodian.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudcustodian.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-custodian/refs/heads/main/security/cloud-custodian-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud Security
- Compliance
- Cost Optimization
- Multi-Cloud
- Policy as Code
---

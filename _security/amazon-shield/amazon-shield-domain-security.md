---
api_specs:
- filename: amazon-shield-openapi.yml
  format: yaml
  label: AWS Shield API
  slug: aws-shield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-openapi.yml
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
- host: shield.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Shield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Shield, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Shield
provider_slug: amazon-shield
slug: amazon-shield-domain-security
source_filename: amazon-shield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: console.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\n- host: shield.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/security/amazon-shield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DDoS Protection
- Networking
- Security
---

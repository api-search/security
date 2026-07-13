---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Lookout for Equipment API
  slug: amazon-lookout-for-equipment-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/lookoutequipment/2020-12-15/openapi.yaml
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
- host: lookoutequipment.amazonaws.com
  https: false
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: lookoutequipment.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Lookout For Equipment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Lookout for Equipment, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Lookout for Equipment
provider_slug: amazon-lookout-for-equipment
slug: amazon-lookout-for-equipment-domain-security
source_filename: amazon-lookout-for-equipment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: lookoutequipment.amazonaws.com\n  https: false\n- host: lookoutequipment.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-equipment/refs/heads/main/security/amazon-lookout-for-equipment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Equipment Monitoring
- Industrial IoT
- Machine Learning
- Predictive Maintenance
---

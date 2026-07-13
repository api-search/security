---
api_specs:
- filename: amazon-iot-greengrass-openapi-original.yml
  format: yaml
  label: AWS IoT Greengrass API
  slug: aws-iot-greengrass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/openapi/amazon-iot-greengrass-openapi-original.yml
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
- host: greengrass.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Iot Greengrass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon IoT Greengrass, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
slug: amazon-iot-greengrass-domain-security
source_filename: amazon-iot-greengrass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: greengrass.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/security/amazon-iot-greengrass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
---

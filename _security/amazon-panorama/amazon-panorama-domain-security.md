---
api_specs:
- filename: amazon-panorama-application-instances-api-openapi.yml
  format: yaml
  label: Amazon Panorama Application Instances API
  slug: amazon-panorama-application-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-application-instances-api-openapi.yml
- filename: amazon-panorama-devices-api-openapi.yml
  format: yaml
  label: Amazon Panorama Devices API
  slug: amazon-panorama-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-devices-api-openapi.yml
- filename: amazon-panorama-jobs-api-openapi.yml
  format: yaml
  label: Amazon Panorama Jobs API
  slug: amazon-panorama-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-jobs-api-openapi.yml
- filename: amazon-panorama-nodes-api-openapi.yml
  format: yaml
  label: Amazon Panorama Nodes API
  slug: amazon-panorama-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-nodes-api-openapi.yml
- filename: amazon-panorama-packages-api-openapi.yml
  format: yaml
  label: Amazon Panorama Packages API
  slug: amazon-panorama-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-packages-api-openapi.yml
- filename: amazon-panorama-tags-api-openapi.yml
  format: yaml
  label: Amazon Panorama Tags API
  slug: amazon-panorama-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/openapi/amazon-panorama-tags-api-openapi.yml
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
- host: panorama.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Panorama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Panorama, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Panorama
provider_slug: amazon-panorama
slug: amazon-panorama-domain-security
source_filename: amazon-panorama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: panorama.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/security/amazon-panorama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
---

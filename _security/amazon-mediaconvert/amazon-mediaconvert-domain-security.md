---
api_specs:
- filename: amazon-mediaconvert-certificates-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Certificates API
  slug: amazon-mediaconvert-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-certificates-api-openapi.yml
- filename: amazon-mediaconvert-endpoints-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Endpoints API
  slug: amazon-mediaconvert-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-endpoints-api-openapi.yml
- filename: amazon-mediaconvert-jobs-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Jobs API
  slug: amazon-mediaconvert-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-jobs-api-openapi.yml
- filename: amazon-mediaconvert-jobtemplates-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert JobTemplates API
  slug: amazon-mediaconvert-jobtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-jobtemplates-api-openapi.yml
- filename: amazon-mediaconvert-policy-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Policy API
  slug: amazon-mediaconvert-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-policy-api-openapi.yml
- filename: amazon-mediaconvert-presets-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Presets API
  slug: amazon-mediaconvert-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-presets-api-openapi.yml
- filename: amazon-mediaconvert-queues-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Queues API
  slug: amazon-mediaconvert-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-queues-api-openapi.yml
- filename: amazon-mediaconvert-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Tags API
  slug: amazon-mediaconvert-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Mediaconvert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon MediaConvert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
slug: amazon-mediaconvert-domain-security
source_filename: amazon-mediaconvert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/security/amazon-mediaconvert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Media Processing
- Media
---

---
api_specs:
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Instances API
  slug: shadeform-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Instance Types & Availability API
  slug: shadeform-instance-types-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Templates API
  slug: shadeform-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Volumes API
  slug: shadeform-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform SSH Keys API
  slug: shadeform-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shadeform.ai
  spf: true
hosts:
- cert_expires: Sep 10 01:10:06 2026 GMT
  host: www.shadeform.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 00:22:48 2026 GMT
  host: docs.shadeform.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 22:35:33 2026 GMT
  host: api.shadeform.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shadeform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shadeform, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shadeform
provider_slug: shadeform
slug: shadeform-domain-security
source_filename: shadeform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shadeform.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:10:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.shadeform.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:22:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.shadeform.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 22:35:33 2026 GMT\n  hsts: null\ndomains:\n- domain: shadeform.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/security/shadeform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GPU
- Cloud
- Marketplace
- Compute
- Infrastructure
- AI
---

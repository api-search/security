---
api_specs:
- filename: blumira-health-api-openapi.yml
  format: yaml
  label: Blumira Health API
  slug: blumira-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-health-api-openapi.yml
- filename: blumira-msp-api-openapi.yml
  format: yaml
  label: Blumira Msp API
  slug: blumira-msp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-msp-api-openapi.yml
- filename: blumira-org-api-openapi.yml
  format: yaml
  label: Blumira Org API
  slug: blumira-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-org-api-openapi.yml
- filename: blumira-resolutions-api-openapi.yml
  format: yaml
  label: Blumira Resolutions API
  slug: blumira-resolutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-resolutions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blumira.com
  spf: true
hosts:
- cert_expires: Nov 12 08:36:14 2026 GMT
  host: www.blumira.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blumira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blumira, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Blumira
provider_slug: blumira
slug: blumira-domain-security
source_filename: blumira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blumira.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 08:36:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blumira.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/security/blumira-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Software-as-a-Service
- Cloud
- IT
---

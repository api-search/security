---
api_specs:
- filename: spectro-cloud-palette-openapi.json
  format: json
  label: Palette APIs
  slug: palette-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/openapi/spectro-cloud-palette-openapi.json
- filename: spectro-cloud-edge-management-openapi.json
  format: json
  label: Edge Local Management APIs
  slug: edge-local-management-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/openapi/spectro-cloud-edge-management-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spectrocloud.com
  spf: true
hosts:
- cert_expires: Sep 23 09:58:48 2026 GMT
  host: spectrocloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.spectrocloud.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spectro Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spectro Cloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spectro Cloud
provider_slug: spectro-cloud
slug: spectro-cloud-domain-security
source_filename: spectro-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spectrocloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:58:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spectrocloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spectrocloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/security/spectro-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure
- Kubernetes
- Cloud Native
- Cluster Management
- Edge Computing
- Multi-Cloud
- DevOps
- AI Infrastructure
---

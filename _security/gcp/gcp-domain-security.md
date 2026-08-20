---
api_specs:
- filename: gcp-disks-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Disks API
  slug: gcp-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-disks-api-openapi.yml
- filename: gcp-firewalls-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Firewalls API
  slug: gcp-firewalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-firewalls-api-openapi.yml
- filename: gcp-images-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Images API
  slug: gcp-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-images-api-openapi.yml
- filename: gcp-instances-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Instances API
  slug: gcp-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-instances-api-openapi.yml
- filename: gcp-machinetypes-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs MachineTypes API
  slug: gcp-machinetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-machinetypes-api-openapi.yml
- filename: gcp-networks-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Networks API
  slug: gcp-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-networks-api-openapi.yml
- filename: gcp-snapshots-api-openapi.yml
  format: yaml
  label: Google Cloud Platform APIs Snapshots API
  slug: gcp-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/openapi/gcp-snapshots-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: compute.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:41:23 2026 GMT
  host: storage.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Platform APIs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Platform APIs
provider_slug: gcp
slug: gcp-domain-security
source_filename: gcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: compute.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: storage.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:41:23 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/security/gcp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine-Learning
- Networking
- Security
- Serverless
- Storage
---

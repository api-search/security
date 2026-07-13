---
api_specs:
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Identification API
  slug: identification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud File Scanning API
  slug: file-scanning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Broadcast Monitoring API
  slug: broadcast-monitoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Buckets & Metadata API
  slug: buckets-metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Console API
  slug: console
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acrcloud.com
  spf: false
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.acrcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 22:14:32 2026 GMT
  host: docs.acrcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: identify-eu-west-1.acrcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Acrcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACRCloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: ACRCloud
provider_slug: acrcloud
slug: acrcloud-domain-security
source_filename: acrcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acrcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.acrcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 22:14:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: identify-eu-west-1.acrcloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: acrcloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/security/acrcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Audio
- Music Recognition
- Audio Fingerprinting
- Broadcast Monitoring
- Metadata
---

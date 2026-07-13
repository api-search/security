---
api_specs:
- filename: allianz-future-cloud-platform-services.yaml
  format: yaml
  label: Allianz Future Cloud Platform Services API
  slug: platform-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/openapi/allianz-future-cloud-platform-services.yaml
- filename: allianz-future-cloud-platform-policy.yaml
  format: yaml
  label: Allianz Insurance Policy Microservice API
  slug: policy-microservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/openapi/allianz-future-cloud-platform-policy.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allianz.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cncf.io
  spf: true
hosts:
- cert_expires: Aug 12 16:58:20 2026 GMT
  host: www.allianz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 20:53:47 2026 GMT
  host: architecture.cncf.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: platform.allianz.com
  https: false
kind: domain-security
layout: security
method: probed
name: Allianz Future Cloud Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allianz Future Cloud Platform, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
slug: allianz-future-cloud-platform-domain-security
source_filename: allianz-future-cloud-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allianz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: architecture.cncf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.allianz.com\n  https: false\ndomains:\n- domain: allianz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cncf.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/security/allianz-future-cloud-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
---

---
api_specs:
- filename: google-kubernetes-engine-openapi.yml
  format: yaml
  label: Google Kubernetes Engine
  slug: google-kubernetes-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-kubernetes-engine/refs/heads/main/openapi/google-kubernetes-engine-openapi.yml
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
- cert_expires: Sep 14 08:41:22 2026 GMT
  host: container.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Kubernetes Engine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Kubernetes Engine, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Kubernetes Engine
provider_slug: google-kubernetes-engine
slug: google-kubernetes-engine-domain-security
source_filename: google-kubernetes-engine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: container.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:41:22 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-kubernetes-engine/refs/heads/main/security/google-kubernetes-engine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- Containers
- Google Cloud
- Kubernetes
- Managed Service
- Orchestration
---

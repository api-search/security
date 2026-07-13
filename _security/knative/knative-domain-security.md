---
api_specs:
- filename: knative-serving-api-openapi.yml
  format: yaml
  label: Knative Serving API
  slug: knative-serving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-serving-api-openapi.yml
- filename: knative-eventing-api-openapi.yml
  format: yaml
  label: Knative Eventing API
  slug: knative-eventing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-eventing-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: knative.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Oct  5 21:03:45 2026 GMT
  host: knative.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
kind: domain-security
layout: security
method: probed
name: Knative Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knative, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Knative
provider_slug: knative
slug: knative-domain-security
source_filename: knative-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knative.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kubernetes.default.svc\n  https: false\ndomains:\n- domain: knative.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/security/knative-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Auto-Scaling
- Cloud Native
- Event-Driven
- Graduated
- Kubernetes
- Serverless
---

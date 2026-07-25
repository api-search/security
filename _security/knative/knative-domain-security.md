---
api_specs:
- filename: knative-apis-api-openapi.yml
  format: yaml
  label: Knative Apis API
  slug: knative-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-apis-api-openapi.yml
- filename: knative-brokers-api-openapi.yml
  format: yaml
  label: Knative Brokers API
  slug: knative-brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-brokers-api-openapi.yml
- filename: knative-channels-api-openapi.yml
  format: yaml
  label: Knative Channels API
  slug: knative-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-channels-api-openapi.yml
- filename: knative-configurations-api-openapi.yml
  format: yaml
  label: Knative Configurations API
  slug: knative-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-configurations-api-openapi.yml
- filename: knative-domainmappings-api-openapi.yml
  format: yaml
  label: Knative DomainMappings API
  slug: knative-domainmappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-domainmappings-api-openapi.yml
- filename: knative-eventsources-api-openapi.yml
  format: yaml
  label: Knative EventSources API
  slug: knative-eventsources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-eventsources-api-openapi.yml
- filename: knative-eventtypes-api-openapi.yml
  format: yaml
  label: Knative EventTypes API
  slug: knative-eventtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-eventtypes-api-openapi.yml
- filename: knative-revisions-api-openapi.yml
  format: yaml
  label: Knative Revisions API
  slug: knative-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-revisions-api-openapi.yml
- filename: knative-routes-api-openapi.yml
  format: yaml
  label: Knative Routes API
  slug: knative-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-routes-api-openapi.yml
- filename: knative-subscriptions-api-openapi.yml
  format: yaml
  label: Knative Subscriptions API
  slug: knative-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-subscriptions-api-openapi.yml
- filename: knative-triggers-api-openapi.yml
  format: yaml
  label: Knative Triggers API
  slug: knative-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-triggers-api-openapi.yml
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

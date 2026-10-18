---
api_specs:
- filename: openfaas-alexellis-api-openapi.yml
  format: yaml
  label: OpenFaaS Alexellis API
  slug: openfaas-alexellis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/openapi/openfaas-alexellis-api-openapi.yml
- filename: openfaas-async-function-api-openapi.yml
  format: yaml
  label: OpenFaaS Async Function API
  slug: openfaas-async-function-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/openapi/openfaas-async-function-api-openapi.yml
- filename: openfaas-auth-api-openapi.yml
  format: yaml
  label: OpenFaaS Auth API
  slug: openfaas-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/openapi/openfaas-auth-api-openapi.yml
- filename: openfaas-function-api-openapi.yml
  format: yaml
  label: OpenFaaS Function API
  slug: openfaas-function-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/openapi/openfaas-function-api-openapi.yml
- filename: openfaas-openfaas-api-api-openapi.yml
  format: yaml
  label: OpenFaaS OpenFaaS API
  slug: openfaas-openfaas-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/openapi/openfaas-openfaas-api-api-openapi.yml
- filename: openfaas-system-api-openapi.yml
  format: yaml
  label: OpenFaaS System API
  slug: openfaas-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/openapi/openfaas-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openfaas.com
  spf: true
hosts:
- cert_expires: Nov 28 23:53:51 2026 GMT
  host: www.openfaas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openfaas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenFaaS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenFaaS
provider_slug: openfaas
slug: openfaas-domain-security
source_filename: openfaas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openfaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:53:51 2026 GMT\n  hsts: false\ndomains:\n- domain: openfaas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/security/openfaas-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Serverless
- Open Source
- Functions
- Kubernetes
---

---
api_specs:
- filename: argocd-server-openapi.json
  format: json
  label: Argo CD Applications API
  slug: argocd-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/openapi/argocd-server-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: argo-cd.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argocd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argo CD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Argo CD
provider_slug: argocd
slug: argocd-domain-security
source_filename: argocd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argo-cd.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argocd/refs/heads/main/security/argocd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- DevOps
- GitOps
- Kubernetes
- Continuous Delivery
- CNCF
- Open Source
- Operator
---

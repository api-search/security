---
api_specs:
- filename: trivy-server-openapi.yml
  format: yaml
  label: Trivy Server API
  slug: trivy-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trivy/refs/heads/main/openapi/trivy-server-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: trivy.dev
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Sep 29 20:29:34 2026 GMT
  host: trivy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
kind: domain-security
layout: security
method: probed
name: Trivy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trivy, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trivy
provider_slug: trivy
slug: trivy-domain-security
source_filename: trivy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trivy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:29:34 2026 GMT\n  hsts: false\n- host: kubernetes.default.svc\n  https: false\ndomains:\n- domain: trivy.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: false\n  dmarc: false\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trivy/refs/heads/main/security/trivy-domain-security.yml
summary_line: TLSv1.3
tags:
- Containers
- Kubernetes
- SBOM
- Security
- Vulnerability Scanning
- Open Source
- DevSecOps
- Cloud Security
---

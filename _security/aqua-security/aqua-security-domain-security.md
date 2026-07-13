---
api_specs:
- filename: aqua-security-api.yaml
  format: yaml
  label: Aqua Security
  slug: aqua-security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/openapi/aqua-security-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aquasec.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: trivy.dev
  spf: false
hosts:
- cert_expires: Sep 14 15:01:53 2026 GMT
  host: www.aquasec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:29:34 2026 GMT
  host: trivy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aqua Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aqua Security, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aqua Security
provider_slug: aqua-security
slug: aqua-security-domain-security
source_filename: aqua-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aquasec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trivy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:29:34 2026 GMT\n  hsts: false\ndomains:\n- domain: aquasec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: trivy.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/security/aqua-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
---

---
api_specs:
- filename: finos-symphony-pod-api-openapi.yml
  format: yaml
  label: Symphony API Spec
  slug: symphony-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finos/refs/heads/main/openapi/finos-symphony-pod-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finos.org
  spf: true
hosts:
- cert_expires: Sep 20 16:59:39 2026 GMT
  host: www.finos.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:02:26 2026 GMT
  host: fdc3.finos.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 17:13:45 2026 GMT
  host: morphir.finos.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FINOS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FINOS
provider_slug: finos
slug: finos-domain-security
source_filename: finos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:59:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fdc3.finos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:02:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: morphir.finos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finos.org\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finos/refs/heads/main/security/finos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Fintech
- Linux Foundation
- Open Source
---

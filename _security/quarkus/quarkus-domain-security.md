---
api_specs:
- filename: quarkus-dev-ui-openapi.yml
  format: yaml
  label: Quarkus
  slug: quarkus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quarkus/refs/heads/main/openapi/quarkus-dev-ui-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quarkus.io
  spf: true
hosts:
- cert_expires: Sep 17 01:15:47 2026 GMT
  host: quarkus.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quarkus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quarkus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quarkus
provider_slug: quarkus
slug: quarkus-domain-security
source_filename: quarkus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quarkus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:15:47 2026 GMT\n  hsts: false\ndomains:\n- domain: quarkus.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quarkus/refs/heads/main/security/quarkus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Native
- Frameworks
- GraalVM
- Java
- Kubernetes
- Microservices
- Serverless
---

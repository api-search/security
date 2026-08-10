---
api_specs:
- filename: skymind-model-upload-api-openapi.yml
  format: yaml
  label: Pathmind Model Upload API
  slug: skymind-model-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skymind/refs/heads/main/openapi/skymind-model-upload-api-openapi.yml
- filename: skymind-projects-api-openapi.yml
  format: yaml
  label: Pathmind Projects API
  slug: skymind-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skymind/refs/heads/main/openapi/skymind-projects-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: pathmind.com
  spf: true
hosts:
- cert_expires: Sep 23 18:02:31 2026 GMT
  host: pathmind.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.pathmind.com
  https: false
kind: domain-security
layout: security
method: probed
name: Skymind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pathmind, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pathmind
provider_slug: skymind
slug: skymind-domain-security
source_filename: skymind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pathmind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:02:31 2026 GMT\n  hsts: null\n- host: api.pathmind.com\n  https: false\ndomains:\n- domain: pathmind.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skymind/refs/heads/main/security/skymind-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Reinforcement Learning
- Simulation
- Optimization
- Supply Chain
- Manufacturing
- Defunct
---

---
api_specs:
- filename: kaedim-web-api-openapi.yml
  format: yaml
  label: Kaedim Web API
  slug: kaedim-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaedim/refs/heads/main/openapi/kaedim-web-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kaedim3d.com
  spf: true
hosts:
- cert_expires: Oct 16 13:44:17 2026 GMT
  host: api.kaedim3d.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaedim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaedim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kaedim
provider_slug: kaedim
slug: kaedim-domain-security
source_filename: kaedim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.kaedim3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 13:44:17 2026 GMT\n  hsts: null\ndomains:\n- domain: kaedim3d.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaedim/refs/heads/main/security/kaedim-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- 3D
- Artificial Intelligence
- Generative AI
- Gaming
- 3D Models
- Asset Generation
- Content Generation
- Machine Learning
---

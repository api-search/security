---
api_specs:
- filename: rhizome-ai-openapi.yml
  format: yaml
  label: Rhizome AI API
  slug: rhizome-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhizome-ai/refs/heads/main/openapi/rhizome-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rhizomeai.com
  spf: true
hosts:
- cert_expires: Sep 27 06:25:01 2026 GMT
  host: rhizomeai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 12:50:21 2026 GMT
  host: docs.rhizomeai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rhizome Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhizome Ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhizome Ai
provider_slug: rhizome-ai
slug: rhizome-ai-domain-security
source_filename: rhizome-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rhizomeai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:25:01 2026 GMT\n  hsts: false\n- host: docs.rhizomeai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 12:50:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rhizomeai.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhizome-ai/refs/heads/main/security/rhizome-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Regulatory
- Pharmaceutical
- Medical Devices
- Life Sciences
- Document Search
- Artificial Intelligence
- Compliance
---

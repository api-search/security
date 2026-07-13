---
api_specs:
- filename: overview
  format: yaml
  label: Torq REST API
  slug: torq-rest-api
  spec_type: OpenAPI
  url: https://developers.torq.io/apidocs/overview
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:security@torq.io"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: torq.io
  spf: true
hosts:
- cert_expires: Sep 14 02:27:27 2026 GMT
  host: torq.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:32:21 2026 GMT
  host: developers.torq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 08:19:25 2026 GMT
  host: api.torq.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Torq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Torq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Torq
provider_slug: torq
slug: torq-domain-security
source_filename: torq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: torq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:27:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.torq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:32:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.torq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:19:25 2026 GMT\n  hsts: null\ndomains:\n- domain: torq.io\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:security@torq.io\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torq/refs/heads/main/security/torq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security Automation
- SOAR
- Hyper-Automation
- Security Orchestration
- Incident Response
- No-Code
- AI SOC
- Workflows
- Playbooks
- Security Operations
---

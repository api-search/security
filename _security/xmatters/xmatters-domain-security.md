---
api_specs:
- filename: xmatters-openapi.yml
  format: yaml
  label: xMatters REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@xmatters.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: xmatters.com
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: www.xmatters.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: help.xmatters.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xmatters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xMatters, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: xMatters
provider_slug: xmatters
slug: xmatters-domain-security
source_filename: xmatters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xmatters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.xmatters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: xmatters.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@xmatters.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/security/xmatters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Incident Management
- On-Call
- Alerting
- Service Reliability
- DevOps
- Communication
- Workflow Automation
---

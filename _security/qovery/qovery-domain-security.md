---
api_specs:
- filename: qovery-openapi.yaml
  format: yaml
  label: Qovery
  slug: qovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qovery/main/openapi/qovery-openapi.yaml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qovery.com
  spf: true
hosts:
- cert_expires: Aug 17 22:26:41 2026 GMT
  host: www.qovery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 22:26:41 2026 GMT
  host: api-doc.qovery.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 06:04:12 2026 GMT
  host: api.qovery.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qovery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qovery, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qovery
provider_slug: qovery
slug: qovery-domain-security
source_filename: qovery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qovery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:26:41 2026 GMT\n  hsts: false\n- host: api-doc.qovery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:26:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.qovery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:04:12 2026 GMT\n  hsts: null\ndomains:\n- domain: qovery.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qovery/refs/heads/main/security/qovery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Deployment
- Developer Experience
- Internal Developer Platform
---

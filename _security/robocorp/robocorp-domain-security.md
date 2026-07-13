---
api_specs:
- filename: openapi.json
  format: json
  label: Robocorp Control Room API
  slug: control-room-api
  spec_type: OpenAPI
  url: https://robocorp.com/api/openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: robocorp.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rpaframework.org
  spf: true
hosts:
- cert_expires: Sep 19 20:17:39 2026 GMT
  host: robocorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: cloud.robocorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 19:06:22 2026 GMT
  host: rpaframework.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robocorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robocorp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Robocorp
provider_slug: robocorp
slug: robocorp-domain-security
source_filename: robocorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.robocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpaframework.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:06:22 2026 GMT\n  hsts: false\ndomains:\n- domain: robocorp.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rpaframework.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/security/robocorp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- RPA
- Workflow Automation
- Python
- Open Source
- Automation
---

---
api_specs:
- filename: dome9-api
  format: yaml
  label: Dome9 API
  slug: dome9-api
  spec_type: Postman
  url: https://www.postman.com/dome9-security/workspace/dome9-api
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: checkpoint.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dome9.com
  spf: true
hosts:
- cert_expires: Jan  2 06:44:08 2027 GMT
  host: www.checkpoint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api-v2-docs.dome9.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.dome9.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dome9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dome9, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dome9
provider_slug: dome9
slug: dome9-domain-security
source_filename: dome9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 06:44:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-v2-docs.dome9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\n- host: api.dome9.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: checkpoint.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dome9.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dome9/refs/heads/main/security/dome9-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Security
- Compliance
- Infrastructure Security
- Multi-Cloud
- Security Posture Management
---

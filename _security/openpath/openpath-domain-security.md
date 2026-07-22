---
api_specs:
- filename: openpath-openapi-original.json
  format: json
  label: Openpath API
  slug: openpath-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/openapi/openpath-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openpath.com
  spf: true
hosts:
- cert_expires: Sep 11 02:54:07 2026 GMT
  host: www.openpath.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.openpath.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openpath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openpath, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Openpath
provider_slug: openpath
slug: openpath-domain-security
source_filename: openpath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:54:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: openpath.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/security/openpath-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Access Control
- Physical Security
- Identity
- Credentials
- IoT
- Smart Building
- Avigilon Alta
- Motorola Solutions
---

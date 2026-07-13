---
api_specs:
- filename: swagger.json
  format: json
  label: CloudGuard CNAPP REST API
  slug: cloudguard-cnapp-api
  spec_type: OpenAPI
  url: https://api.dome9.com/v2/swagger.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: checkpoint.com
  spf: true
hosts:
- cert_expires: Jan  2 06:44:08 2027 GMT
  host: www.checkpoint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 09:25:52 2026 GMT
  host: docs.cgn.portal.checkpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: sc1.checkpoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudGuard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CloudGuard
provider_slug: cloudguard
slug: cloudguard-domain-security
source_filename: cloudguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 06:44:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cgn.portal.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 09:25:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sc1.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: checkpoint.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudguard/refs/heads/main/security/cloudguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Check Point
- CNAPP
- Cloud Security
- Compliance
- CSPM
- CWPP
- Posture Management
---

---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: devexpress.com
  spf: true
hosts:
- cert_expires: Mar 31 21:05:29 2027 GMT
  host: devexpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Devexpress Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for devexpress-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: devexpress-com
provider_slug: devexpress-com
slug: devexpress-com-domain-security
source_filename: devexpress-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 21:05:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: devexpress.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/devexpress-com/security/devexpress-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- UI Controls
- Developer Tools
- .NET
- JavaScript
---

---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "globalsign.com"
  - 0 iodef "mailto:jai.sharma@infoedge.com"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: naukri.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: naukri.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Naukri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Naukri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Naukri
provider_slug: naukri
slug: naukri-domain-security
source_filename: naukri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: naukri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: naukri.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 iodef \"mailto:jai.sharma@infoedge.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/naukri/security/naukri-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Jobs
- Recruitment
- Career
- India
---

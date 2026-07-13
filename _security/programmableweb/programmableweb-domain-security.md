---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:caa-violations@salesforce.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: programmableweb.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archive.org
  spf: true
hosts:
- host: www.programmableweb.com
  https: false
- cert_expires: Feb  9 22:02:42 2027 GMT
  host: web.archive.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Programmableweb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProgrammableWeb, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ProgrammableWeb
provider_slug: programmableweb
slug: programmableweb-domain-security
source_filename: programmableweb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.programmableweb.com\n  https: false\n- host: web.archive.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 22:02:42 2027 GMT\n  hsts: false\ndomains:\n- domain: programmableweb.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:caa-violations@salesforce.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: archive.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/programmableweb/refs/heads/main/security/programmableweb-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- API Aggregation
- API Directory
- API Discovery
- Archived
- Developer Resources
- Mashups
---

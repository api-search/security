---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: icndb.com
  spf: false
hosts:
- cert_expires: Sep  3 13:43:54 2026 GMT
  host: www.icndb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chuck Norris Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chuck Norris Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Chuck Norris Database
provider_slug: chuck-norris-database
slug: chuck-norris-database-domain-security
source_filename: chuck-norris-database-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icndb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 13:43:54 2026 GMT\n  hsts: false\ndomains:\n- domain: icndb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chuck-norris-database/refs/heads/main/security/chuck-norris-database-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---

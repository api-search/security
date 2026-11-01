---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kayaposoft.com
  spf: true
hosts:
- cert_expires: Jan 22 18:21:23 2027 GMT
  host: kayaposoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Enrico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enrico holiday service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Enrico holiday service
provider_slug: enrico
slug: enrico-domain-security
source_filename: enrico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kayaposoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 18:21:23 2027 GMT\n  hsts: false\ndomains:\n- domain: kayaposoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/enrico/security/enrico-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Holiday
- API
- Slovakia
- OpenSource
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nothingunseen.com
  spf: true
hosts:
- cert_expires: Jan 28 13:03:54 2027 GMT
  host: nothingunseen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nothing Unseen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nothing Unseen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nothing Unseen
provider_slug: nothingunseen-com
slug: nothingunseen-com-domain-security
source_filename: nothingunseen-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nothingunseen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 13:03:54 2027 GMT\n  hsts: false\ndomains:\n- domain: nothingunseen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nothingunseen-com/security/nothingunseen-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Search
- Transparency
- Legal
- Data
- Open Source
---

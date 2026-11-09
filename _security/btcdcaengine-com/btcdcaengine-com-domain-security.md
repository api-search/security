---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: btcdcaengine.com
  spf: false
hosts:
- cert_expires: Jan 20 06:40:23 2027 GMT
  host: btcdcaengine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Btcdcaengine Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BTC DCA Engine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BTC DCA Engine
provider_slug: btcdcaengine-com
slug: btcdcaengine-com-domain-security
source_filename: btcdcaengine-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: btcdcaengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 06:40:23 2027 GMT\n  hsts: false\ndomains:\n- domain: btcdcaengine.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/btcdcaengine-com/security/btcdcaengine-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Bitcoin
- DCA
- Calculator
- Finance
- Cryptocurrency
---

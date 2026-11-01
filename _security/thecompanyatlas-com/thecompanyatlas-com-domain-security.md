---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thecompanyatlas.com
  spf: true
hosts:
- cert_expires: Dec 28 14:16:42 2026 GMT
  host: thecompanyatlas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thecompanyatlas Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for thecompanyatlas-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: thecompanyatlas-com
provider_slug: thecompanyatlas-com
slug: thecompanyatlas-com-domain-security
source_filename: thecompanyatlas-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thecompanyatlas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 14:16:42 2026 GMT\n  hsts: false\ndomains:\n- domain: thecompanyatlas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/thecompanyatlas-com/security/thecompanyatlas-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Customs
- TradeData
- API
- DataPlatform
---

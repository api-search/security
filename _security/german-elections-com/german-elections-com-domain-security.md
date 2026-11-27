---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: german-elections.com
  spf: true
hosts:
- cert_expires: Dec 28 17:10:22 2026 GMT
  host: german-elections.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 'GERDA: German Election Database Domain Security'
name_suffix: Domain Security
overview: 'Domain security posture for GERDA: German Election Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 'GERDA: German Election Database'
provider_slug: german-elections-com
slug: german-elections-com-domain-security
source_filename: german-elections-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: german-elections.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 17:10:22 2026 GMT\n  hsts: false\ndomains:\n- domain: german-elections.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/german-elections-com/security/german-elections-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Elections
- Germany
- Data
- Open Data
---

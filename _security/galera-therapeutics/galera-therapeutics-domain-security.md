---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: galeratx.com
  spf: true
hosts:
- cert_expires: Dec 31 03:41:42 2026 GMT
  host: www.galeratx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Galera Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galera Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Galera Therapeutics
provider_slug: galera-therapeutics
slug: galera-therapeutics-domain-security
source_filename: galera-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.galeratx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 03:41:42 2026 GMT\n  hsts: false\ndomains:\n- domain: galeratx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/galera-therapeutics/security/galera-therapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

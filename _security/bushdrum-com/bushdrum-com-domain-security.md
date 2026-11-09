---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bushdrum.com
  spf: true
hosts:
- cert_expires: Jan 11 17:32:07 2027 GMT
  host: bushdrum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bushdrum Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bushdrum-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: bushdrum-com
provider_slug: bushdrum-com
slug: bushdrum-com-domain-security
source_filename: bushdrum-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bushdrum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 17:32:07 2027 GMT\n  hsts: false\ndomains:\n- domain: bushdrum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bushdrum-com/security/bushdrum-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

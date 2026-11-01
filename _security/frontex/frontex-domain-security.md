---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: europa.eu
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.frontex.europa.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Frontex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FRONTEX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FRONTEX
provider_slug: frontex
slug: frontex-domain-security
source_filename: frontex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frontex.europa.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: europa.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/frontex/security/frontex-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Border Management
- European Union
- Security
- Government
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vectoralix.com
  spf: false
hosts:
- cert_expires: Jan 11 18:28:01 2027 GMT
  host: vectoralix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vectoralix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectoralix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vectoralix
provider_slug: vectoralix
slug: vectoralix-domain-security
source_filename: vectoralix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vectoralix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 18:28:01 2027 GMT\n  hsts: null\ndomains:\n- domain: vectoralix.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/vectoralix/security/vectoralix-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---

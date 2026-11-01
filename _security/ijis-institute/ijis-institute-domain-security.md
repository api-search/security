---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ijis.org
  spf: true
hosts:
- cert_expires: Jan 21 09:22:18 2027 GMT
  host: www.ijis.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ijis Institute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IJIS Institute, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IJIS Institute
provider_slug: ijis-institute
slug: ijis-institute-domain-security
source_filename: ijis-institute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ijis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 09:22:18 2027 GMT\n  hsts: null\ndomains:\n- domain: ijis.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ijis-institute/security/ijis-institute-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---

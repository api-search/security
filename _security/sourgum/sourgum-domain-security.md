---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sourgum.com
  spf: true
hosts:
- cert_expires: May  5 23:59:59 2027 GMT
  host: www.sourgum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sourgum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourgum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sourgum
provider_slug: sourgum
slug: sourgum-domain-security
source_filename: sourgum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sourgum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sourgum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sourgum/security/sourgum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Waste Management
- Recycling
- Technology
- Sustainability
---

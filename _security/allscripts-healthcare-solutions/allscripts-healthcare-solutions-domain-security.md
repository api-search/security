---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: allscripts.com
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: www.allscripts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.allscripts.com
  https: false
- host: api.allscripts.com
  https: false
kind: domain-security
layout: security
method: probed
name: Allscripts Healthcare Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allscripts Healthcare Solutions, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Allscripts Healthcare Solutions
provider_slug: allscripts-healthcare-solutions
slug: allscripts-healthcare-solutions-domain-security
source_filename: allscripts-healthcare-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allscripts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.allscripts.com\n  https: false\n- host: api.allscripts.com\n  https: false\ndomains:\n- domain: allscripts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allscripts-healthcare-solutions/refs/heads/main/security/allscripts-healthcare-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare IT
- EHR
- Clinical
---

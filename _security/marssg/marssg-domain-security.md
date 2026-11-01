---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: marssg.com
  spf: true
hosts:
- cert_expires: Nov 22 13:27:59 2026 GMT
  host: marssg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marssg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MARS Solutions Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MARS Solutions Group
provider_slug: marssg
slug: marssg-domain-security
source_filename: marssg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marssg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 13:27:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: marssg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/marssg/security/marssg-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Recruiting
- Artificial Intelligence
- TalentSolutions
- Staffing
---

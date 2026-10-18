---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: benkitechnologies.com
  spf: true
hosts:
- cert_expires: Nov 30 12:55:10 2026 GMT
  host: www.benkitechnologies.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ben Ki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Benki
provider_slug: ben-ki
slug: ben-ki-domain-security
source_filename: ben-ki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benkitechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 12:55:10 2026 GMT\n  hsts: false\ndomains:\n- domain: benkitechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ben-ki/refs/heads/main/security/ben-ki-domain-security.yml
summary_line: TLSv1.3
tags:
- Software
- IT Consulting
- Artificial Intelligence
- GIS
- Services
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rcsaustralia.com.au
  spf: true
hosts:
- cert_expires: Jan 19 08:50:00 2027 GMT
  host: rcsaustralia.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rcs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RCS (Resource Consulting Services), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RCS (Resource Consulting Services)
provider_slug: rcs
slug: rcs-domain-security
source_filename: rcs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rcsaustralia.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 08:50:00 2027 GMT\n  hsts: false\ndomains:\n- domain: rcsaustralia.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/rcs/security/rcs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agriculture
- Consulting
- Training
- Professional-Development
- Australia
---

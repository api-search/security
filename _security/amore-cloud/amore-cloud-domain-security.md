---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amore.cloud
  spf: false
hosts:
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: amore.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amore Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starberg & More Solutions AB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Starberg & More Solutions AB
provider_slug: amore-cloud
slug: amore-cloud-domain-security
source_filename: amore-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amore.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: amore.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amore-cloud/security/amore-cloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IT Consulting
- Artificial Intelligence
- Integration
- Software Development
- Sweden
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heyspark.co
  spf: true
hosts:
- cert_expires: Jan  4 21:31:30 2027 GMT
  host: heyspark.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HeySpark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeySpark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HeySpark
provider_slug: heyspark-co
slug: heyspark-co-domain-security
source_filename: heyspark-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heyspark.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 21:31:30 2027 GMT\n  hsts: false\ndomains:\n- domain: heyspark.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heyspark-co/security/heyspark-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web Development
- Small Business
- AI Integration
- Custom Websites
---

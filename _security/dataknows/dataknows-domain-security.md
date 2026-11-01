---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dataknows.ai
  spf: true
hosts:
- cert_expires: May  1 23:59:59 2027 GMT
  host: www.dataknows.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dataknows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dataknows, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dataknows
provider_slug: dataknows
slug: dataknows-domain-security
source_filename: dataknows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dataknows.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: May  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dataknows.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dataknows/security/dataknows-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Artificial Intelligence
- Real Estate
- Data Analytics
- Advertising
- B2B
---

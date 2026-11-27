---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lead411.com
  spf: false
hosts:
- cert_expires: Feb 12 05:50:02 2027 GMT
  host: lead411.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lead411 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lead411, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lead411
provider_slug: lead411-com
slug: lead411-com-domain-security
source_filename: lead411-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lead411.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 05:50:02 2027 GMT\n  hsts: false\ndomains:\n- domain: lead411.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lead411-com/security/lead411-com-domain-security.yml
summary_line: TLSv1.3
tags:
- B2B
- Sales
- Marketing
- Data
- Lead Enrichment
---

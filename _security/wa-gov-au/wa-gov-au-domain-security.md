---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wa.gov.au
  spf: true
hosts:
- cert_expires: Jan  4 06:53:51 2027 GMT
  host: wamex.dmp.wa.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Department of Local Government, Industry Regulation and Safety Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Local Government, Industry Regulation and Safety, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Department of Local Government, Industry Regulation and Safety
provider_slug: wa-gov-au
slug: wa-gov-au-domain-security
source_filename: wa-gov-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wamex.dmp.wa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 06:53:51 2027 GMT\n  hsts: null\ndomains:\n- domain: wa.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wa-gov-au/security/wa-gov-au-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Western Australia
- Regulations
- Safety
- Licensing
- Company
---

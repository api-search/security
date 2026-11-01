---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aidatanorge.no
  spf: true
hosts:
- cert_expires: Jan 21 22:57:30 2027 GMT
  host: aidatanorge.no
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aidatanorge No Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aidatanorge-no, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aidatanorge-no
provider_slug: aidatanorge-no
slug: aidatanorge-no-domain-security
source_filename: aidatanorge-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aidatanorge.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 22:57:30 2027 GMT\n  hsts: false\ndomains:\n- domain: aidatanorge.no\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aidatanorge-no/security/aidatanorge-no-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- AI
- Data
- Nordic
---

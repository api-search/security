---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ftnnetwork.com
  spf: false
hosts:
- cert_expires: Jan  5 18:15:32 2027 GMT
  host: ftnnetwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ftnnetwork Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FTN Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: FTN Network
provider_slug: ftnnetwork-com
slug: ftnnetwork-com-domain-security
source_filename: ftnnetwork-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ftnnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 18:15:32 2027 GMT\n  hsts: false\ndomains:\n- domain: ftnnetwork.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ftnnetwork-com/security/ftnnetwork-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Networking
- API
- Enterprise
- Security
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: makerreels.com
  spf: false
hosts:
- cert_expires: Feb 13 04:42:55 2027 GMT
  host: makerreels.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MakerReels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MakerReels, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: MakerReels
provider_slug: makerreels-com
slug: makerreels-com-domain-security
source_filename: makerreels-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makerreels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 04:42:55 2027 GMT\n  hsts: false\ndomains:\n- domain: makerreels.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/makerreels-com/security/makerreels-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Artificial Intelligence
- Mobile
- UGC
---

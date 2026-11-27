---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: teppi.xyz
  spf: true
hosts:
- cert_expires: Jan 27 02:08:31 2027 GMT
  host: teppi.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teppi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teppi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teppi
provider_slug: teppi-xyz
slug: teppi-xyz-domain-security
source_filename: teppi-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teppi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 02:08:31 2027 GMT\n  hsts: false\ndomains:\n- domain: teppi.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/teppi-xyz/security/teppi-xyz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- Monitoring
- Transparency
- Data
---

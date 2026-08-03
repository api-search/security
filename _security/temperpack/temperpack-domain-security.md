---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: temperpack.com
  spf: true
hosts:
- cert_expires: Oct 25 23:57:58 2026 GMT
  host: www.temperpack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Temperpack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TemperPack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TemperPack
provider_slug: temperpack
slug: temperpack-domain-security
source_filename: temperpack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.temperpack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:57:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: temperpack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temperpack/refs/heads/main/security/temperpack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Packaging
- Sustainable Packaging
- Cold Chain
- Logistics
- Supply Chain
- Manufacturing
- Life Sciences
- Food and Beverage
- Materials
---

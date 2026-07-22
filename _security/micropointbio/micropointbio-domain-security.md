---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: micropointbio.com.cn
  spf: false
hosts:
- cert_expires: Jul 28 05:42:39 2026 GMT
  host: micropointbio.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Micropointbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for micropointbio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: micropointbio
provider_slug: micropointbio
slug: micropointbio-domain-security
source_filename: micropointbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: micropointbio.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 05:42:39 2026 GMT\n  hsts: false\ndomains:\n- domain: micropointbio.com.cn\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micropointbio/refs/heads/main/security/micropointbio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Biotechnology
- Medical Devices
- Diagnostics
- POCT
- In Vitro Diagnostics
- Biochips
- Microfluidics
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nextsilicon.com
  spf: true
hosts:
- cert_expires: Sep 23 06:10:48 2026 GMT
  host: www.nextsilicon.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nextsilicon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NextSilicon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NextSilicon
provider_slug: nextsilicon
slug: nextsilicon-domain-security
source_filename: nextsilicon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextsilicon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:10:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: nextsilicon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextsilicon/refs/heads/main/security/nextsilicon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compute
- High Performance Computing
- Semiconductors
- Hardware
- Accelerators
- RISC-V
- Artificial Intelligence
---

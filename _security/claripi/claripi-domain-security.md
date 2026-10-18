---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: claripi.com
  spf: true
hosts:
- cert_expires: Nov 10 03:23:39 2026 GMT
  host: claripi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claripi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claripi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Claripi
provider_slug: claripi
slug: claripi-domain-security
source_filename: claripi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claripi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 03:23:39 2026 GMT\n  hsts: false\ndomains:\n- domain: claripi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claripi/refs/heads/main/security/claripi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Imaging
- Artificial Intelligence
- Healthcare
- Software
---

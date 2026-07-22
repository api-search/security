---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kerys.software
  spf: true
hosts:
- cert_expires: Sep 17 16:39:25 2026 GMT
  host: kerys.software
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kerys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kerys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kerys
provider_slug: kerys
slug: kerys-domain-security
source_filename: kerys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kerys.software\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:39:25 2026 GMT\n  hsts: null\ndomains:\n- domain: kerys.software\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kerys/refs/heads/main/security/kerys-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Virtualization
- Type 1 Hypervisor
- Endpoint Security
- Secure Workstation
- OT Security
- Compliance
- France
---

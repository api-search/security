---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gvisor.dev
  spf: true
hosts:
- cert_expires: Oct  2 05:03:31 2026 GMT
  host: gvisor.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gvisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gVisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: gVisor
provider_slug: gvisor
slug: gvisor-domain-security
source_filename: gvisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gvisor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:03:31 2026 GMT\n  hsts: false\ndomains:\n- domain: gvisor.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gvisor/refs/heads/main/security/gvisor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Containers
- Kernel
- Linux
- Open Source
- Sandboxing
- Security
---

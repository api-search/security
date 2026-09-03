---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viaphoton.com
  spf: true
hosts:
- cert_expires: Oct 11 12:01:35 2026 GMT
  host: viaphoton.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viaphoton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for viaPhoton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: viaPhoton
provider_slug: viaphoton
slug: viaphoton-domain-security
source_filename: viaphoton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: viaphoton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 12:01:35 2026 GMT\n  hsts: false\ndomains:\n- domain: viaphoton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viaphoton/refs/heads/main/security/viaphoton-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fiber Optics
- Telecommunications
- Networking
- Data Centers
- Broadband
- Manufacturing
- Hardware
- Connectivity
- 5G
---

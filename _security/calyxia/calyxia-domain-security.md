---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: calyxia.com
  spf: true
hosts:
- cert_expires: Dec 21 13:31:04 2026 GMT
  host: calyxia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calyxia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calyxia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Calyxia
provider_slug: calyxia
slug: calyxia-domain-security
source_filename: calyxia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calyxia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 13:31:04 2026 GMT\n  hsts: false\ndomains:\n- domain: calyxia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calyxia/refs/heads/main/security/calyxia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Microencapsulation
- Advanced Materials
- Agriculture
- Consumer Care
- Home & Beauty
- Sustainable Chemistry
---

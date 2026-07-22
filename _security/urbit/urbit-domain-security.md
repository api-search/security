---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbit.org
  spf: true
hosts:
- cert_expires: Sep  1 20:16:40 2026 GMT
  host: urbit.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 22:14:06 2026 GMT
  host: docs.urbit.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 18:40:14 2026 GMT
  host: roller.urbit.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urbit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Urbit
provider_slug: urbit
slug: urbit-domain-security
source_filename: urbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.urbit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: roller.urbit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:40:14 2026 GMT\n  hsts: null\ndomains:\n- domain: urbit.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbit/refs/heads/main/security/urbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Personal Servers
- Decentralized Identity
- Peer-to-Peer
- Operating Systems
- Self-Hosting
- Agents
---

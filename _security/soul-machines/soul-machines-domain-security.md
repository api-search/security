---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soulmachines.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soulmachines.cloud
  spf: true
hosts:
- cert_expires: Sep 29 08:40:15 2026 GMT
  host: www.soulmachines.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: docs.soulmachines.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 04:20:01 2026 GMT
  host: dh.soulmachines.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soul Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soul Machines, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Soul Machines
provider_slug: soul-machines
slug: soul-machines-domain-security
source_filename: soul-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soulmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:40:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs.soulmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dh.soulmachines.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:20:01 2026 GMT\n  hsts: null\ndomains:\n- domain: soulmachines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: soulmachines.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soul-machines/refs/heads/main/security/soul-machines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Artificial Intelligence
- Digital Humans
- Avatars
- Conversational AI
- Customer Experience
- SDK
- Web SDK
---

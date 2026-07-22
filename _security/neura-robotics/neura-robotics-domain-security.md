---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neura-robotics.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: neuraverse.com
  spf: false
hosts:
- cert_expires: Oct  1 17:26:59 2026 GMT
  host: neura-robotics.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 10:48:10 2026 GMT
  host: neuraverse.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neura Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NEURA Robotics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NEURA Robotics
provider_slug: neura-robotics
slug: neura-robotics-domain-security
source_filename: neura-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neura-robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:26:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: neuraverse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: neura-robotics.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: neuraverse.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neura-robotics/refs/heads/main/security/neura-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Humanoid Robots
- Cognitive Robotics
- Artificial Intelligence
- Automation
- Deep Tech
- Cobots
---

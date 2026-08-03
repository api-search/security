---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cscgeneration.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backcountry.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: seattlecoffeegear.com
  spf: true
hosts:
- cert_expires: Sep 24 10:48:36 2026 GMT
  host: www.cscgeneration.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.backcountry.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 00:46:24 2026 GMT
  host: api.firmly.online
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 09:00:02 2026 GMT
  host: www.seattlecoffeegear.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Csc Generation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CSC Generation, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CSC Generation
provider_slug: csc-generation
slug: csc-generation-domain-security
source_filename: csc-generation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cscgeneration.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:48:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.backcountry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.firmly.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 00:46:24 2026 GMT\n  hsts: null\n- host: www.seattlecoffeegear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 09:00:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: cscgeneration.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: backcountry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: seattlecoffeegear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csc-generation/refs/heads/main/security/csc-generation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Agent Commerce
- Artificial Intelligence
- Universal Commerce Protocol
- Model Context Protocol
- Holding Company
- Shopping
---

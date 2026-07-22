---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vera.com
  spf: true
hosts:
- cert_expires: Sep 10 12:23:56 2026 GMT
  host: www.vera.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vera
provider_slug: vera
slug: vera-domain-security
source_filename: vera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vera.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 12:23:56 2026 GMT\n  hsts: null\ndomains:\n- domain: vera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vera/refs/heads/main/security/vera-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Cybersecurity
- Data Security
- Encryption
- Digital Rights Management
- Information Rights Management
- Secure Collaboration
---

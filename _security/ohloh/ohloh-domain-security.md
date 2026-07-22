---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openhub.net
  spf: true
hosts:
- cert_expires: Aug 22 18:14:46 2026 GMT
  host: www.openhub.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ohloh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ohloh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ohloh
provider_slug: ohloh
slug: ohloh-domain-security
source_filename: ohloh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openhub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:14:46 2026 GMT\n  hsts: null\ndomains:\n- domain: openhub.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ohloh/refs/heads/main/security/ohloh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Open Source
- Open Source Directory
- Code Analytics
- Software Composition
- Developer Data
- Projects
- Contributors
- Black Duck
---

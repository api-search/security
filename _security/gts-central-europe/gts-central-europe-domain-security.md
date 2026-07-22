---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gts.ro
  spf: true
hosts:
- cert_expires: Nov 13 07:06:37 2026 GMT
  host: www.gts.ro
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gts Central Europe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GTS Central Europe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GTS Central Europe
provider_slug: gts-central-europe
slug: gts-central-europe-domain-security
source_filename: gts-central-europe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gts.ro\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 13 07:06:37 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: gts.ro\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gts-central-europe/refs/heads/main/security/gts-central-europe-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Telecommunications
- Cloud
- Cyber Security
- Connectivity
- Managed Services
- Unified Communications
- Romania
---

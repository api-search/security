---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beyondmeat.com
  spf: true
hosts:
- cert_expires: Sep 24 16:59:44 2026 GMT
  host: www.beyondmeat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beyond Meat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beyond Meat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beyond Meat
provider_slug: beyond-meat
slug: beyond-meat-domain-security
source_filename: beyond-meat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beyondmeat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:59:44 2026 GMT\n  hsts: false\ndomains:\n- domain: beyondmeat.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-meat/refs/heads/main/security/beyond-meat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Food
- Plant-Based
- CPG
- Sustainability
- Retail
---

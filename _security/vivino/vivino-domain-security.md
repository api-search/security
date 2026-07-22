---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vivino.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.vivino.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vivino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vivino, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: vivino
provider_slug: vivino
slug: vivino-domain-security
source_filename: vivino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vivino.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vivino.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivino/refs/heads/main/security/vivino-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wine
- Marketplace
- E-Commerce
- Mobile App
- Ratings and Reviews
- Food and Beverage
- Consumer
---

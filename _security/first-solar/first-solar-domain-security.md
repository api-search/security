---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "godaddy.com"
  - 0 issue "www.digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firstsolar.com
  spf: true
hosts:
- cert_expires: Sep 21 20:41:45 2026 GMT
  host: www.firstsolar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Solar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Solar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: First Solar
provider_slug: first-solar
slug: first-solar-domain-security
source_filename: first-solar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstsolar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:41:45 2026 GMT\n  hsts: false\ndomains:\n- domain: firstsolar.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-solar/refs/heads/main/security/first-solar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Solar
- Energy
- Renewable Energy
- Manufacturing
- Fortune 1000
---

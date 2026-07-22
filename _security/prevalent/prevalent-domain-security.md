---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prevalent.net
  spf: true
hosts:
- cert_expires: Sep 30 18:31:11 2026 GMT
  host: www.prevalent.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prevalent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prevalent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prevalent
provider_slug: prevalent
slug: prevalent-domain-security
source_filename: prevalent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prevalent.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:31:11 2026 GMT\n  hsts: false\ndomains:\n- domain: prevalent.net\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prevalent/refs/heads/main/security/prevalent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- Third-Party Risk Management
- TPRM
- Vendor Risk
- Governance Risk Compliance
---

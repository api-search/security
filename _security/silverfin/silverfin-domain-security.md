---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: silverfin.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getsilverfin.com
  spf: true
hosts:
- cert_expires: Aug 28 12:20:15 2026 GMT
  host: silverfin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:46:32 2026 GMT
  host: developer.silverfin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 10:01:32 2026 GMT
  host: live.getsilverfin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silverfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silverfin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Silverfin
provider_slug: silverfin
slug: silverfin-domain-security
source_filename: silverfin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silverfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:20:15 2026 GMT\n  hsts: null\n- host: developer.silverfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:46:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: live.getsilverfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:01:32 2026 GMT\n  hsts: null\ndomains:\n- domain: silverfin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getsilverfin.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverfin/refs/heads/main/security/silverfin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business Applications
- Accounting
- Financial Close
- Bookkeeping
- Reporting
- Compliance
- Fintech
- SaaS
- Belgium
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stash.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stashinvest.com
  spf: true
hosts:
- cert_expires: Aug 27 04:59:57 2026 GMT
  host: www.stash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 14:53:01 2026 GMT
  host: api.stashinvest.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stash, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stash
provider_slug: stash
slug: stash-domain-security
source_filename: stash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 04:59:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stashinvest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 14:53:01 2026 GMT\n  hsts: null\ndomains:\n- domain: stash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stashinvest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stash/refs/heads/main/security/stash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Investing
- Banking
- Fractional Shares
- Portfolio Management
- Financial Education
- Robo-Advisor
- Stock-Back
- Custodial Accounts
- IRA
---

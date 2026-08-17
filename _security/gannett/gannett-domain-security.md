---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "www.digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usatodayco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gannett.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usatoday.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: localiq.com
  spf: true
hosts:
- cert_expires: Sep 22 11:43:22 2026 GMT
  host: www.usatodayco.com
  hsts: false
  https: true
  role: corporate site
  tls_version: TLSv1.3
- cert_expires: Oct 27 22:59:50 2026 GMT
  host: www.gannett.com
  hsts: false
  https: true
  role: legacy corporate host, 301s to www.usatodayco.com
  tls_version: TLSv1.3
- cert_expires: Oct 31 06:54:24 2026 GMT
  host: www.usatoday.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: flagship consumer property
  tls_version: TLSv1.3
- cert_expires: Sep 30 10:19:16 2026 GMT
  host: localiq.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  https: true
  role: LocaliQ digital marketing services
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gannett Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gannett, probed live across 4 host(s) and 4 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gannett
provider_slug: gannett
slug: gannett-domain-security
source_filename: gannett-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Gannett / USA TODAY Co. / LocaliQ host in apis.yml\nnote: >-\n  0-working/probe-domain-security.py covers the single Website host; the remaining three\n  hosts were probed by hand with the same checks (HTTP HEAD for HSTS, openssl s_client for\n  TLS version and cert expiry, dig for DS/CAA/TXT). www.gannett.com is retained because it\n  still serves the 301s into www.usatodayco.com.\nhosts:\n  - host: www.usatodayco.com\n    role: corporate site\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 22 11:43:22 2026 GMT\n    hsts: false\n  - host: www.gannett.com\n    role: legacy corporate host, 301s to www.usatodayco.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Oct 27 22:59:50 2026 GMT\n    hsts: false\n  - host: www.usatoday.com\n    role: flagship consumer property\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Oct 31 06:54:24 2026 GMT\n    hsts:\
  \ true\n    hsts_max_age: 63072000\n  - host: localiq.com\n    role: LocaliQ digital marketing services\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 30 10:19:16 2026 GMT\n    hsts: true\n    hsts_max_age: 2592000\n    hsts_include_subdomains: true\ndomains:\n  - domain: usatodayco.com\n    dnssec: false\n    caa:\n      - 0 issue \"letsencrypt.org\"\n      - 0 issue \"www.digicert.com\"\n      - 0 issue \"amazon.com\"\n    spf: true\n    dmarc: true\n    dmarc_policy: none\n  - domain: gannett.com\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: none\n  - domain: usatoday.com\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: none\n  - domain: localiq.com\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: none\nsummary:\n  https_everywhere: true\n  tls13_everywhere: true\n  hsts_hosts: 2\n  hsts_missing: [www.usatodayco.com, www.gannett.com]\n  dnssec_domains: 0\n  caa_domains:\
  \ 1\n  dmarc_enforcing: 0\n  note: >-\n    All four domains publish SPF with a -all hard fail and a DMARC record, but every DMARC\n    policy is p=none — monitoring only, no enforcement. Only the new corporate domain\n    (usatodayco.com) publishes CAA; the flagship consumer domain usatoday.com does not, and\n    no domain is DNSSEC-signed. The corporate hosts are the only ones without HSTS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gannett/refs/heads/main/security/gannett-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- News
- Publishing
- Journalism
- Digital Marketing
- Advertising
- Local Marketing
- Content
---

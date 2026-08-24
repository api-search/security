---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jswonemsme.com
  note: DMARC published at p=none (monitor only), rua=dmarc-reports@jswonemsme.com. No CAA record.
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jswonehomes.com
  note: No SPF TXT record and no DNSSEC DS record. DMARC reports route to dmarc-reports@jswonemsme.com, confirming shared operation with the marketplace domain.
  spf: false
hosts:
- cert_expires: Oct 30 17:42:32 2026 GMT
  host: www.jswonemsme.com
  hsts: false
  https: true
  note: No Strict-Transport-Security header observed on the JSW One MSME marketplace host.
  tls_version: TLSv1.3
- cert_expires: Oct 10 05:14:41 2026 GMT
  host: www.jswonehomes.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jsw One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JSW One, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: JSW One
provider_slug: jsw-one
slug: jsw-one-domain-security
source_filename: jsw-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every JSW One consumer web host (no API host exists to probe)\nhosts:\n- host: www.jswonemsme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 17:42:32 2026 GMT\n  hsts: false\n  note: No Strict-Transport-Security header observed on the JSW One MSME marketplace host.\n- host: www.jswonehomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:14:41 2026 GMT\n  hsts: true\n  hsts_header: max-age=31536000; includeSubDomains; preload\ndomains:\n- domain: jswonemsme.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: DMARC published at p=none (monitor only), rua=dmarc-reports@jswonemsme.com. No CAA record.\n- domain: jswonehomes.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  note: No SPF TXT record and no DNSSEC DS record. DMARC reports route to dmarc-reports@jswonemsme.com,\n    confirming\
  \ shared operation with the marketplace domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jsw-one/refs/heads/main/security/jsw-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- B2B Commerce
- Marketplace
- Construction
- Steel
- Building Materials
- Manufacturing
- Supply Chain
- Embedded Finance
- MSME
- India
- E-Commerce
---

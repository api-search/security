---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mrcooper.com
  spf: true
hosts:
- cert_expires: Oct  5 20:30:13 2026 GMT
  host: www.mrcooper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nationstar Mortgage Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nationstar Mortgage Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nationstar Mortgage Holdings
provider_slug: nationstar-mortgage-holdings
slug: nationstar-mortgage-holdings-domain-security
source_filename: nationstar-mortgage-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mrcooper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:30:13 2026 GMT\n  hsts: null\ndomains:\n- domain: mrcooper.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationstar-mortgage-holdings/refs/heads/main/security/nationstar-mortgage-holdings-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Mortgage
- Financial Services
- Loan Servicing
- Fortune 1000
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: standardeconomics.com
  spf: true
hosts:
- cert_expires: Oct  9 17:09:11 2026 GMT
  host: www.standardeconomics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Standard Economics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard Economics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Standard Economics
provider_slug: standard-economics
slug: standard-economics-domain-security
source_filename: standard-economics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.standardeconomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:09:11 2026 GMT\n  hsts: false\ndomains:\n- domain: standardeconomics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-economics/refs/heads/main/security/standard-economics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fintech
- Financial Inclusion
- Capital Allocation
- Artificial Intelligence
- Venture Backed
---

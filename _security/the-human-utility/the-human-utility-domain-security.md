---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: detroitwaterproject.org
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.detroitwaterproject.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: The Human Utility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Human Utility, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: The Human Utility
provider_slug: the-human-utility
slug: the-human-utility-domain-security
source_filename: the-human-utility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.detroitwaterproject.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: detroitwaterproject.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-human-utility/refs/heads/main/security/the-human-utility-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Non-Profit
- Water
- Utilities
- Social Impact
- Crowdfunding
- Civic Tech
- Y Combinator
---

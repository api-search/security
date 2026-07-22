---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: axcelius.com
  spf: true
hosts:
- cert_expires: Sep 24 16:35:16 2026 GMT
  host: axcelius.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Axcelius I Ii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axcelius I/II, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Axcelius I/II
provider_slug: axcelius-i-ii
slug: axcelius-i-ii-domain-security
source_filename: axcelius-i-ii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axcelius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 16:35:16 2026 GMT\n  hsts: false\ndomains:\n- domain: axcelius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axcelius-i-ii/refs/heads/main/security/axcelius-i-ii-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Venture Capital
- Company Creation
- Biopharmaceutical
- Life Sciences
- Drug Discovery
- Oncology
- Rare Disease
- Neurodegenerative Disease
- Stealth
---

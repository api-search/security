---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diversyfund.com
  spf: true
hosts:
- cert_expires: Oct 25 16:18:40 2026 GMT
  host: diversyfund.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diversyfund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DiversyFund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DiversyFund
provider_slug: diversyfund
slug: diversyfund-domain-security
source_filename: diversyfund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diversyfund.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 16:18:40 2026 GMT\n  hsts: null\ndomains:\n- domain: diversyfund.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diversyfund/refs/heads/main/security/diversyfund-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real-Estate
- Investing
- Private Markets
- Fixed Income
- Fintech
- Wealth Management
- Crowdfunding
---

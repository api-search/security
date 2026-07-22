---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moonfare.com
  spf: true
hosts:
- cert_expires: Oct  4 08:44:19 2026 GMT
  host: www.moonfare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moonfare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moonfare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moonfare
provider_slug: moonfare
slug: moonfare-domain-security
source_filename: moonfare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moonfare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:44:19 2026 GMT\n  hsts: false\ndomains:\n- domain: moonfare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonfare/refs/heads/main/security/moonfare-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Private Equity
- Venture Capital
- Fintech
- Investing
- Wealth Management
- Alternative Investments
- Financial Services
---

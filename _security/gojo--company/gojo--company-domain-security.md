---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gojo.co
  spf: true
hosts:
- cert_expires: Sep 29 09:49:42 2026 GMT
  host: gojo.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gojo  Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gojo & Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gojo & Company
provider_slug: gojo--company
slug: gojo--company-domain-security
source_filename: gojo--company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gojo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:49:42 2026 GMT\n  hsts: false\ndomains:\n- domain: gojo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojo--company/refs/heads/main/security/gojo--company-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial-Services
- Financial Inclusion
- Microfinance
- Impact Investing
- Holding Company
- Emerging Markets
- Japan
---

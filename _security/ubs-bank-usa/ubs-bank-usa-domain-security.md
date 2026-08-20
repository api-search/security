---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ubs.com
  spf: true
hosts:
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: www.ubs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubs Bank Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UBS Bank USA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: UBS Bank USA
provider_slug: ubs-bank-usa
slug: ubs-bank-usa-domain-security
source_filename: ubs-bank-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ubs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ubs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubs-bank-usa/refs/heads/main/security/ubs-bank-usa-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Wealth Management
- Industrial Bank
- Securities-Based Lending
- Private Banking
---

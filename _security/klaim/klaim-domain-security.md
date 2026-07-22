---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: klaim.ai
  spf: true
hosts:
- cert_expires: Oct  3 09:04:23 2026 GMT
  host: klaim.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klaim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klaim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Klaim
provider_slug: klaim
slug: klaim-domain-security
source_filename: klaim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klaim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:04:23 2026 GMT\n  hsts: false\ndomains:\n- domain: klaim.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaim/refs/heads/main/security/klaim-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fintech
- Healthcare
- Insurance
- Claims
- Invoice Financing
- Working Capital
- Receivables
- Embedded Finance
- Real Estate
- United Arab Emirates
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: westboundequity.com
  spf: true
hosts:
- cert_expires: Sep 16 08:36:09 2026 GMT
  host: westboundequity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Westbound Equity Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Westbound Equity Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Westbound Equity Partners
provider_slug: westbound-equity-partners
slug: westbound-equity-partners-domain-security
source_filename: westbound-equity-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: westboundequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:36:09 2026 GMT\n  hsts: false\ndomains:\n- domain: westboundequity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/westbound-equity-partners/refs/heads/main/security/westbound-equity-partners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Venture Capital
- Investment
- Climate Tech
- Artificial Intelligence
- Social Impact
- Workplace Equity
---

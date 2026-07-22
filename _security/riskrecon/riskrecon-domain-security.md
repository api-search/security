---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: riskrecon.com
  spf: true
hosts:
- cert_expires: Sep 16 21:27:00 2026 GMT
  host: www.riskrecon.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.riskrecon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riskrecon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RiskRecon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: RiskRecon
provider_slug: riskrecon
slug: riskrecon-domain-security
source_filename: riskrecon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.riskrecon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:27:00 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: api.riskrecon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: riskrecon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riskrecon/refs/heads/main/security/riskrecon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Security Ratings
- Third Party Risk
- Supply Chain Risk
- Risk Management
- GRC
- Vendor Monitoring
- Attack Surface
---

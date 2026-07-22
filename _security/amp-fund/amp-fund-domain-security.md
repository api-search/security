---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amppublic.com
  spf: false
hosts:
- cert_expires: Oct  8 17:42:31 2026 GMT
  host: www.amppublic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amp Fund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMP Fund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: AMP Fund
provider_slug: amp-fund
slug: amp-fund-domain-security
source_filename: amp-fund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amppublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:42:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amppublic.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amp-fund/refs/heads/main/security/amp-fund-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Compute
- Infrastructure
- Venture Capital
- Public Benefit Corporation
- Data Centers
- GPU
---

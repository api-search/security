---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pvxpartners.com
  spf: true
hosts:
- cert_expires: Aug 26 07:33:03 2026 GMT
  host: www.pvxpartners.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pvx Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pvx Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pvx Partners
provider_slug: pvx-partners
slug: pvx-partners-domain-security
source_filename: pvx-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pvxpartners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pvxpartners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pvx-partners/refs/heads/main/security/pvx-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financing
- User Acquisition
- Mobile Gaming
- Consumer Apps
- Analytics
- Venture Debt
---

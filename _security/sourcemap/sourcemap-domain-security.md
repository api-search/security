---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sourcemap.com
  spf: true
hosts:
- cert_expires: Oct 14 02:06:00 2026 GMT
  host: www.sourcemap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 16:33:39 2026 GMT
  host: api.sourcemap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourcemap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourcemap, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sourcemap
provider_slug: sourcemap
slug: sourcemap-domain-security
source_filename: sourcemap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sourcemap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 02:06:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sourcemap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 16:33:39 2026 GMT\n  hsts: null\ndomains:\n- domain: sourcemap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcemap/refs/heads/main/security/sourcemap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Supply Chain
- Traceability
- Supply Chain Transparency
- Due Diligence
- Regulatory Compliance
- ESG
- Sustainability
- Risk Management
- Logistics
- Manufacturing
---

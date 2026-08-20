---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:pt-systems-support@rea-group.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: proptrack.com.au
  spf: true
hosts:
- cert_expires: Sep  2 17:47:29 2026 GMT
  host: www.proptrack.com.au
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:33:34 2026 GMT
  host: developer.proptrack.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proptrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PropTrack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PropTrack
provider_slug: proptrack
slug: proptrack-domain-security
source_filename: proptrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proptrack.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:47:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.proptrack.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: proptrack.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:pt-systems-support@rea-group.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proptrack/refs/heads/main/security/proptrack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Property Data
- Real-Estate
- Automated Valuation
- Property Valuation
- Australia
- Market Data
- Data & Analytics
- PropTech
---

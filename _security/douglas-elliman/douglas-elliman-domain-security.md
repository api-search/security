---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elliman.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.elliman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  3 17:31:36 2027 GMT
  host: api.elliman.com
  hsts: false
  hsts_max_age: null
  https: true
  note: Private IIS/ASP.NET host. HTTP 403 at root, no anonymous access, no documentation. Probed for transport posture only; it is not a listed API.
  tls_version: TLSv1.2
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: status.elliman.com
  hsts: false
  hsts_max_age: null
  https: true
  note: Self-hosted Uptime Kuma behind nginx/1.24.0 (Ubuntu). Root 302s to /dashboard (login-gated); no public status page is published. See lifecycle/.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Douglas Elliman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Douglas Elliman, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Douglas Elliman
provider_slug: douglas-elliman
slug: douglas-elliman-domain-security
source_filename: douglas-elliman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + known Douglas Elliman subdomains\nhosts:\n- host: www.elliman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.elliman.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  3 17:31:36 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Private IIS/ASP.NET host. HTTP 403 at root, no anonymous access, no documentation.\n    Probed for transport posture only; it is not a listed API.\n- host: status.elliman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Self-hosted Uptime Kuma behind nginx/1.24.0 (Ubuntu). Root 302s to /dashboard\n    (login-gated); no public status page is published. See lifecycle/.\ndomains:\n- domain: elliman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/douglas-elliman/refs/heads/main/security/douglas-elliman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United States
- Brokerage
- Property Listings
- MLS
- IDX
- RESO
- Rentals
- Commercial Real Estate
- Property Management
- Title
- Escrow
- PropTech
- Luxury Real Estate
- New Development
---

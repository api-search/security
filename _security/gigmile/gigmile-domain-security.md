---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gigmile.com
  spf: false
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: gigmile.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gigmile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gigmile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gigmile
provider_slug: gigmile
slug: gigmile-domain-security
source_filename: gigmile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gigmile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gigmile.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigmile/refs/heads/main/security/gigmile-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Mobility
- Fintech
- Vehicle Financing
- Gig Economy
- Ride-hailing
- Lease-to-own
- Earned Wage Access
- Insurance
- Africa
---

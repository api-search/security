---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fridayflightdeals.com
  spf: true
hosts:
- cert_expires: Dec 19 20:31:33 2026 GMT
  host: fridayflightdeals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Friday Flight Deals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Friday Flight Deals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Friday Flight Deals
provider_slug: fridayflightdeals-com
slug: fridayflightdeals-com-domain-security
source_filename: fridayflightdeals-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fridayflightdeals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 20:31:33 2026 GMT\n  hsts: false\ndomains:\n- domain: fridayflightdeals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fridayflightdeals-com/security/fridayflightdeals-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Flights
- Deals
- Travel
- Email
- Weekly
- Company
---

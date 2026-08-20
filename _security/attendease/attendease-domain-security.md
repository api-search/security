---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eventupplanner.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: attendease.com
  spf: true
hosts:
- cert_expires: Oct 16 13:40:09 2026 GMT
  host: eventupplanner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: developer.attendease.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: your-org.attendease.org
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Attendease Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attendease, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Attendease
provider_slug: attendease
slug: attendease-domain-security
source_filename: attendease-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventupplanner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 13:40:09 2026 GMT\n  hsts: false\n- host: developer.attendease.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\n- host: your-org.attendease.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: eventupplanner.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: attendease.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attendease/refs/heads/main/security/attendease-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Event
- Event Management
- Event Marketing
- Conferences
- Webinars
- Attendees
- Registration
- Software-as-a-Service
---

---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetblue.com
  spf: true
hosts:
- cert_expires: Sep 26 02:43:03 2026 GMT
  host: www.jetblue.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 02:43:03 2026 GMT
  host: accounts.jetblue.com
  hsts: true
  hsts_max_age: 300
  https: true
  note: Okta-hosted identity provider; serves the OIDC + RFC 8414 discovery documents.
  tls_version: TLSv1.3
- cert_expires: Sep 26 02:43:03 2026 GMT
  host: api.jetblue.com
  hsts: true
  hsts_max_age: 300
  https: true
  note: Fastly-fronted internal edge host; HTTP 404 at every probed path.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetblue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JetBlue, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JetBlue
provider_slug: jetblue
slug: jetblue-domain-security
source_filename: jetblue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: accounts.jetblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n  note: Okta-hosted identity provider; serves the OIDC + RFC 8414 discovery documents.\n- host: api.jetblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n  note: Fastly-fronted internal edge host; HTTP 404 at every probed path.\ndomains:\n- domain: jetblue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetblue/refs/heads/main/security/jetblue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United States
- Aviation
- Airline
- Distribution
- NDC
- GDS
- Booking
- Loyalty
---

---
description: ''
domains:
- caa:
  - 0 iodef "mailto:AAbdulj@bart.gov"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bart.gov
  spf: true
hosts:
- cert_expires: Sep 19 20:14:43 2026 GMT
  host: api.bart.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bay Area Rapid Transit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bay Area Rapid Transit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bay Area Rapid Transit
provider_slug: bay-area-rapid-transit
slug: bay-area-rapid-transit-domain-security
source_filename: bay-area-rapid-transit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.bart.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:14:43 2026 GMT\n  hsts: false\ndomains:\n- domain: bart.gov\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:AAbdulj@bart.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bay-area-rapid-transit/refs/heads/main/security/bay-area-rapid-transit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ip2country.info
  spf: false
hosts:
- cert_expires: Oct  5 00:01:47 2026 GMT
  host: ip2country.info
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ip 2 Country Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IP 2 Country, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: IP 2 Country
provider_slug: ip-2-country
slug: ip-2-country-domain-security
source_filename: ip-2-country-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ip2country.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:01:47 2026 GMT\n  hsts: false\ndomains:\n- domain: ip2country.info\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ip-2-country/refs/heads/main/security/ip-2-country-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---

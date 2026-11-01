---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: extreme-ip-lookup.com
  spf: true
hosts:
- cert_expires: Jan 17 09:57:04 2027 GMT
  host: extreme-ip-lookup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Extreme Ip Lookup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extreme IP Lookup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Extreme IP Lookup
provider_slug: extreme-ip-lookup
slug: extreme-ip-lookup-domain-security
source_filename: extreme-ip-lookup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extreme-ip-lookup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 09:57:04 2027 GMT\n  hsts: false\ndomains:\n- domain: extreme-ip-lookup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/extreme-ip-lookup/security/extreme-ip-lookup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geolocation
- IP
- API
- Data
- Netherlands
---

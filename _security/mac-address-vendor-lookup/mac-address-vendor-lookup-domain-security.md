---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: macaddress.io
  spf: true
hosts:
- cert_expires: Oct  3 10:16:36 2026 GMT
  host: macaddress.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mac Address Vendor Lookup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MAC address vendor lookup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MAC address vendor lookup
provider_slug: mac-address-vendor-lookup
slug: mac-address-vendor-lookup-domain-security
source_filename: mac-address-vendor-lookup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: macaddress.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:16:36 2026 GMT\n  hsts: false\ndomains:\n- domain: macaddress.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mac-address-vendor-lookup/refs/heads/main/security/mac-address-vendor-lookup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- Public APIs
---

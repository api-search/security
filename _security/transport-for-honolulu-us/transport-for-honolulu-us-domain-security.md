---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thebus.org
  spf: true
hosts:
- cert_expires: Oct 25 22:06:00 2026 GMT
  host: hea.thebus.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Honolulu Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Honolulu, US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Transport for Honolulu, US
provider_slug: transport-for-honolulu-us
slug: transport-for-honolulu-us-domain-security
source_filename: transport-for-honolulu-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hea.thebus.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 22:06:00 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: thebus.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-honolulu-us/refs/heads/main/security/transport-for-honolulu-us-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Transportation
- Public APIs
---

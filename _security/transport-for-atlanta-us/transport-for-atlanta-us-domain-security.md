---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: itsmarta.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.itsmarta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Atlanta Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Atlanta, US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transport for Atlanta, US
provider_slug: transport-for-atlanta-us
slug: transport-for-atlanta-us-domain-security
source_filename: transport-for-atlanta-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itsmarta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: itsmarta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-atlanta-us/refs/heads/main/security/transport-for-atlanta-us-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---

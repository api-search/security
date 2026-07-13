---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: json2jsonp.com
  spf: false
hosts:
- cert_expires: Sep  2 19:47:00 2026 GMT
  host: json2jsonp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Json 2 Jsonp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JSON 2 JSONP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: JSON 2 JSONP
provider_slug: json-2-jsonp
slug: json-2-jsonp-domain-security
source_filename: json-2-jsonp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: json2jsonp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 19:47:00 2026 GMT\n  hsts: false\ndomains:\n- domain: json2jsonp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/json-2-jsonp/refs/heads/main/security/json-2-jsonp-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---

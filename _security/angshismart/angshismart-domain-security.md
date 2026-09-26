---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: angshigroup.com
  spf: true
hosts:
- cert_expires: Dec 19 18:32:19 2026 GMT
  host: www.angshigroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Angshismart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angshismart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Angshismart
provider_slug: angshismart
slug: angshismart-domain-security
source_filename: angshismart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.angshigroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 18:32:19 2026 GMT\n  hsts: false\ndomains:\n- domain: angshigroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angshismart/refs/heads/main/security/angshismart-domain-security.yml
summary_line: TLSv1.3
tags:
- Manufacturing
- Pharmaceuticals
- China
- Enterprise
- Angshi
---

---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: myip.com
  spf: true
hosts:
- cert_expires: Oct  7 20:19:50 2026 GMT
  host: www.myip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: My Ip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MY IP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MY IP
provider_slug: my-ip
slug: my-ip-domain-security
source_filename: my-ip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:19:50 2026 GMT\n  hsts: false\ndomains:\n- domain: myip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/my-ip/refs/heads/main/security/my-ip-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---

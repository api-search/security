---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: privoxy.org
  spf: true
hosts:
- cert_expires: Sep 29 12:22:23 2026 GMT
  host: www.privoxy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Privoxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Privoxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Privoxy
provider_slug: privoxy
slug: privoxy-domain-security
source_filename: privoxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.privoxy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:22:23 2026 GMT\n  hsts: false\ndomains:\n- domain: privoxy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privoxy/refs/heads/main/security/privoxy-domain-security.yml
summary_line: TLSv1.3
tags:
- Privacy Proxy
- Proxy
---

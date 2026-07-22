---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: liangyihui.net
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.liangyihui.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: api.liangyihui.net
  hsts: false
  https: true
  notes: private first-party API host; root returns Tomcat "Welcome to LYH!", server header Tengine
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liangyihui Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for liangyihui, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: liangyihui
provider_slug: liangyihui
slug: liangyihui-domain-security
source_filename: liangyihui-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liangyihui.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n- host: api.liangyihui.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n  notes: private first-party API host; root returns Tomcat \"Welcome to LYH!\", server\n    header Tengine\ndomains:\n- domain: liangyihui.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liangyihui/refs/heads/main/security/liangyihui-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- China
- Venture Backed
- Qiming Portfolio
- Private API
- No Public API Program
---

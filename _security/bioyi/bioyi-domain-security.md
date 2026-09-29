---
description: ''
domains:
- caa:
  - meiguo.ytaotao.net.
  dmarc: false
  dnssec: true
  domain: bioyi.com
  spf: false
hosts:
- host: bioyi.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bioyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bioyi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Bioyi
provider_slug: bioyi
slug: bioyi-domain-security
source_filename: bioyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bioyi.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: bioyi.com\n  dnssec: true\n  caa:\n  - meiguo.ytaotao.net.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioyi/refs/heads/main/security/bioyi-domain-security.yml
summary_line: DNSSEC
tags:
- Company
---

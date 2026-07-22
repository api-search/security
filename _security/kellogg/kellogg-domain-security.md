---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kellogg.com
  spf: true
hosts:
- host: www.kellogg.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.kellogg'
kind: domain-security
layout: security
method: probed
name: Kellogg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kellogg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kellogg
provider_slug: kellogg
slug: kellogg-domain-security
source_filename: kellogg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kellogg.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.kellogg'\n  hsts: null\ndomains:\n- domain: kellogg.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kellogg/refs/heads/main/security/kellogg-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Consumer Packaged Goods
- Cereal
- Food
- Fortune 500
---

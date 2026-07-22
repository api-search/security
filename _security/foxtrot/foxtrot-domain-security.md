---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foxtrotco.com
  spf: true
hosts:
- host: www.foxtrotco.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.foxtrot'
kind: domain-security
layout: security
method: probed
name: Foxtrot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foxtrot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Foxtrot
provider_slug: foxtrot
slug: foxtrot-domain-security
source_filename: foxtrot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxtrotco.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.foxtrot'\n  hsts: null\ndomains:\n- domain: foxtrotco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foxtrot/refs/heads/main/security/foxtrot-domain-security.yml
summary_line: DMARC
tags:
- Company
- Retail
- Convenience Store
- Cafe
- Grocery
- Food and Beverage
- Ecommerce
- Chicago
---

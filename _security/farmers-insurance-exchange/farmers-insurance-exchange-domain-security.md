---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: farmersinsurance.com
  spf: true
hosts:
- host: www.farmersinsurance.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.farmers'
kind: domain-security
layout: security
method: probed
name: Farmers Insurance Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmers Insurance Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Farmers Insurance Exchange
provider_slug: farmers-insurance-exchange
slug: farmers-insurance-exchange-domain-security
source_filename: farmers-insurance-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.farmersinsurance.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.farmers'\n  hsts: null\ndomains:\n- domain: farmersinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmers-insurance-exchange/refs/heads/main/security/farmers-insurance-exchange-domain-security.yml
summary_line: DMARC
tags:
- Fortune 500
- Insurance
---

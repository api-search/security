---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: downstreamimpact.com
  spf: true
hosts:
- host: downstreamimpact.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''downstreami'
kind: domain-security
layout: security
method: probed
name: Downstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Downstream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Downstream
provider_slug: downstream
slug: downstream-domain-security
source_filename: downstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: downstreamimpact.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''downstreami'\n  hsts: null\ndomains:\n- domain: downstreamimpact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/downstream/refs/heads/main/security/downstream-domain-security.yml
summary_line: DMARC
tags:
- Company
- Amazon Advertising
- Retail Media
- Ecommerce
- Advertising Technology
- Marketing Analytics
- SaaS
- Acquired
---

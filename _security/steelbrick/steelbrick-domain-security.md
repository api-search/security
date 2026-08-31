---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steelbrick.com
  spf: false
hosts:
- host: www.steelbrick.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.steelbr'
kind: domain-security
layout: security
method: probed
name: Steelbrick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steelbrick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Steelbrick
provider_slug: steelbrick
slug: steelbrick-domain-security
source_filename: steelbrick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.steelbrick.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.steelbr'\n  hsts: null\ndomains:\n- domain: steelbrick.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steelbrick/refs/heads/main/security/steelbrick-domain-security.yml
summary_line: DMARC
tags:
- Company
- Enterprise Saas
- CPQ
- Configure Price Quote
- Quote To Cash
- Sales
- Acquired
- Salesforce
---

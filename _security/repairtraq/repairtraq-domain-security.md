---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: repairtraq.com
  spf: true
hosts:
- host: repairtraq.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''repairtraq.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Repairtraq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upland Consulting Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Upland Consulting Group
provider_slug: repairtraq
slug: repairtraq-domain-security
source_filename: repairtraq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: repairtraq.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''repairtraq.'\n  hsts: null\ndomains:\n- domain: repairtraq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/repairtraq/security/repairtraq-domain-security.yml
summary_line: DMARC
tags:
- Company
- Consulting
- Repair
- Tracking
- Management
---

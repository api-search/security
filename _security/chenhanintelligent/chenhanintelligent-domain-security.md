---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: morninghan.com
  spf: true
hosts:
- host: www.morninghan.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.morning'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chenhanintelligent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chenhanintelligent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chenhanintelligent
provider_slug: chenhanintelligent
slug: chenhanintelligent-domain-security
source_filename: chenhanintelligent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.morninghan.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.morning'\n  hsts: null\ndomains:\n- domain: morninghan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chenhanintelligent/refs/heads/main/security/chenhanintelligent-domain-security.yml
summary_line: DMARC
tags:
- Company
- Intelligent Cockpit
- Electric Vehicles
- Hardware
- Software
---

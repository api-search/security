---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: breathelife.com
  spf: true
hosts:
- host: www.breathelife.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.breathe'
kind: domain-security
layout: security
method: probed
name: Breathe Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breathe Life, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Breathe Life
provider_slug: breathe-life
slug: breathe-life-domain-security
source_filename: breathe-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breathelife.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.breathe'\n  hsts: null\ndomains:\n- domain: breathelife.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breathe-life/refs/heads/main/security/breathe-life-domain-security.yml
summary_line: DMARC
tags:
- Insurance
- Canada
- Life Insurance
- Insurtech
- Core Systems
- Policy Origination
- Quoting
- Underwriting
- Agent Tools
- SaaS
- Acquired
---

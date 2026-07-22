---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: morf.health
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: morf.healthcare
  spf: false
hosts:
- cert_expires: Sep 30 02:30:06 2026 GMT
  host: morf.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.morf.health
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''docs.morf.h'
- cert_expires: Oct 17 22:59:02 2026 GMT
  host: api.morf.healthcare
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morf, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Morf
provider_slug: morf
slug: morf-domain-security
source_filename: morf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morf.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:30:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.morf.health\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''docs.morf.h'\n  hsts: null\n- host: api.morf.healthcare\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 22:59:02 2026 GMT\n  hsts: null\ndomains:\n- domain: morf.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: morf.healthcare\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morf/refs/heads/main/security/morf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health IT
- Automation
- Integration
- iPaaS
- Webhooks
- EHR
- Patient Communication
- HIPAA
- Workflow
- Digital Health
---

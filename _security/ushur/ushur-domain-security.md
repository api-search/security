---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ushur.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ushur.me
  spf: false
hosts:
- cert_expires: Oct 10 06:12:51 2026 GMT
  host: ushur.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ushur.me
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ushur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ushur, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ushur
provider_slug: ushur
slug: ushur-domain-security
source_filename: ushur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ushur.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:12:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ushur.me\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ushur.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ushur.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ushur/refs/heads/main/security/ushur-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Customer Experience
- Automation
- Healthcare
- Insurance
- Financial Services
- Agents
---

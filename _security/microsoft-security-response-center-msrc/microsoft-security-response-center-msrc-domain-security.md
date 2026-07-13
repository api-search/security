---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 17 16:33:21 2026 GMT
  host: msrc.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Security Response Center Msrc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Security Response Center (MSRC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Security Response Center (MSRC)
provider_slug: microsoft-security-response-center-msrc
slug: microsoft-security-response-center-msrc-domain-security
source_filename: microsoft-security-response-center-msrc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: msrc.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 16:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-security-response-center-msrc/refs/heads/main/security/microsoft-security-response-center-msrc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Public APIs
---

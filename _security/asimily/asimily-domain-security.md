---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: asimily.com
  spf: true
hosts:
- cert_expires: Nov 13 08:53:09 2026 GMT
  host: asimily.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asimily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asimily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Asimily
provider_slug: asimily
slug: asimily-domain-security
source_filename: asimily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asimily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 08:53:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: asimily.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asimily/refs/heads/main/security/asimily-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- IoT
- Cybersecurity
- Asset Management
- Risk Modeling
---

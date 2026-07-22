---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: neverware.com
  spf: true
hosts:
- cert_expires: Sep 21 08:42:04 2026 GMT
  host: www.neverware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neverware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neverware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Neverware
provider_slug: neverware
slug: neverware-domain-security
source_filename: neverware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neverware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:42:04 2026 GMT\n  hsts: false\ndomains:\n- domain: neverware.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neverware/refs/heads/main/security/neverware-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Operating System
- ChromeOS
- Endpoint Management
- Device Refurbishment
- Acquired
---

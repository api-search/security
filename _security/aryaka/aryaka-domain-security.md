---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aryaka.com
  spf: true
hosts:
- cert_expires: Oct  7 05:19:44 2026 GMT
  host: www.aryaka.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 14:36:56 2026 GMT
  host: docs.aryaka.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 34560000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 18:00:59 2026 GMT
  host: my.aryaka.com
  hsts: false
  https: true
  note: MyAryaka customer portal, fronted by Cloudflare; returns 403 to non-browser clients.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aryaka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aryaka, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aryaka
provider_slug: aryaka
slug: aryaka-domain-security
source_filename: aryaka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aryaka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 05:19:44 2026 GMT\n  hsts: false\n- host: docs.aryaka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:36:56 2026 GMT\n  hsts: true\n  hsts_max_age: 34560000\n  hsts_include_subdomains: true\n- host: my.aryaka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:00:59 2026 GMT\n  hsts: false\n  note: MyAryaka customer portal, fronted by Cloudflare; returns 403 to non-browser clients.\ndomains:\n- domain: aryaka.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aryaka/refs/heads/main/security/aryaka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- SASE
- SD-WAN
- Network Security
- Zero Trust
- ZTNA
- Cloud Connectivity
- Managed Services
- Firewall
- Secure Web Gateway
- WAN Optimization
- Multi-Cloud
- Telecommunications
---

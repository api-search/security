---
description: ''
domains:
- caa:
  - shunt-h5.wdfangyi.com.
  - shunt-h5-fy06svb1.wdfangyi.com.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: weidian.com
  spf: true
hosts:
- cert_expires: Nov 24 03:21:04 2026 GMT
  host: www.weidian.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Weidan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weidan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Weidan
provider_slug: weidan
slug: weidan-domain-security
source_filename: weidan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weidian.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 03:21:04 2026 GMT\n  hsts: false\ndomains:\n- domain: weidian.com\n  dnssec: true\n  caa:\n  - shunt-h5.wdfangyi.com.\n  - shunt-h5-fy06svb1.wdfangyi.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/weidan/security/weidan-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
---

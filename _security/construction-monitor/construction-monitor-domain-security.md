---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: constructionmonitor.com
  spf: true
hosts:
- cert_expires: Aug 26 12:28:48 2026 GMT
  host: www.constructionmonitor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Construction Monitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Construction Monitor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Construction Monitor
provider_slug: construction-monitor
slug: construction-monitor-domain-security
source_filename: construction-monitor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.constructionmonitor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 12:28:48 2026 GMT\n  hsts: false\ndomains:\n- domain: constructionmonitor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/construction-monitor/refs/heads/main/security/construction-monitor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Contractors
- Lead Generation
- Permits
- Real Estate
---

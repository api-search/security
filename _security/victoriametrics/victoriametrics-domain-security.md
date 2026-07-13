---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@victoriametrics.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: victoriametrics.com
  spf: true
hosts:
- cert_expires: Aug 23 02:46:41 2026 GMT
  host: victoriametrics.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 05:24:42 2026 GMT
  host: docs.victoriametrics.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Victoriametrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VictoriaMetrics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: VictoriaMetrics
provider_slug: victoriametrics
slug: victoriametrics-domain-security
source_filename: victoriametrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: victoriametrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:46:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: docs.victoriametrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 05:24:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: victoriametrics.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@victoriametrics.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victoriametrics/refs/heads/main/security/victoriametrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Database
- Time-Series
- Monitoring
- Open Source
- Prometheus
- PromQL
- MetricsQL
- Observability
---

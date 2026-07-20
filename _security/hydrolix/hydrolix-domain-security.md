---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hydrolix.io
  spf: true
hosts:
- cert_expires: Oct  6 05:25:05 2026 GMT
  host: hydrolix.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hydrolix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydrolix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hydrolix
provider_slug: hydrolix
slug: hydrolix-domain-security
source_filename: hydrolix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hydrolix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:25:05 2026 GMT\n  hsts: false\ndomains:\n- domain: hydrolix.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrolix/refs/heads/main/security/hydrolix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Observability
- Log Analytics
- Data Lake
- Streaming
- ClickHouse
- Monitoring
- Time Series
---

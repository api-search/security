---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: groundcover.com
  spf: true
hosts:
- cert_expires: Oct 12 06:41:53 2026 GMT
  host: www.groundcover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 21:30:08 2026 GMT
  host: docs.groundcover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.groundcover.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groundcover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groundcover, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Groundcover
provider_slug: groundcover
slug: groundcover-domain-security
source_filename: groundcover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.groundcover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 06:41:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.groundcover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 21:30:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.groundcover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: groundcover.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundcover/refs/heads/main/security/groundcover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Observability
- Kubernetes
- eBPF
- Monitoring
- Logs
- Traces
- Metrics
- OpenTelemetry
- MCP
---

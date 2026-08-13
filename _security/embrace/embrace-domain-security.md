---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@embrace.io"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: embrace.io
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: embrace.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 01:42:52 2026 GMT
  host: api.embrace.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 01:42:52 2026 GMT
  host: mcp.embrace.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Embrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Embrace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Embrace
provider_slug: embrace
slug: embrace-domain-security
source_filename: embrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: embrace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.embrace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:42:52 2026 GMT\n  hsts: null\n- host: mcp.embrace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:42:52 2026 GMT\n  hsts: null\ndomains:\n- domain: embrace.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@embrace.io\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embrace/refs/heads/main/security/embrace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Observability
- Monitoring
- Mobile
- Real User Monitoring
- OpenTelemetry
- Metrics
- Crash Reporting
- Application Performance Monitoring
- Developer Tools
- Model Context Protocol
---

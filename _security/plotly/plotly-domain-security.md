---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:webmaster@plotly.com"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plotly.com
  spf: true
hosts:
- cert_expires: Nov 23 04:55:39 2026 GMT
  host: plotly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 01:01:14 2026 GMT
  host: dash.plotly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plotly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plotly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plotly
provider_slug: plotly
slug: plotly-domain-security
source_filename: plotly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plotly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 04:55:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dash.plotly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 01:01:14 2026 GMT\n  hsts: false\ndomains:\n- domain: plotly.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:webmaster@plotly.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plotly/refs/heads/main/security/plotly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Visualization
- Analytics
- Data Apps
- Business Intelligence
- Open Source
- Python
- JavaScript
- Charts
- Dashboards
- Developer Tools
- MCP
---

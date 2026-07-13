---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 iodef "mailto:security@mendix.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mendix.com
  spf: true
hosts:
- cert_expires: Sep 29 10:46:19 2026 GMT
  host: www.mendix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: docs.mendix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: deploy.mendix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mendix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mendix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mendix
provider_slug: mendix
slug: mendix-domain-security
source_filename: mendix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mendix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:46:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mendix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: deploy.mendix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mendix.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:security@mendix.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/security/mendix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Low-Code
- Application Development
- Enterprise Platform
- Application Lifecycle
- Deployment
- Governance
---

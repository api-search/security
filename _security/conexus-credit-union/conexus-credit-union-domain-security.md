---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@conexus.ca"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conexus.ca
  spf: true
hosts:
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: www.conexus.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conexus Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conexus Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Conexus Credit Union
provider_slug: conexus-credit-union
slug: conexus-credit-union-domain-security
source_filename: conexus-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conexus.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conexus.ca\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@conexus.ca\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conexus-credit-union/refs/heads/main/security/conexus-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Credit Union
- Cooperative
- Saskatchewan
- Data Aggregation
- Open Banking
---

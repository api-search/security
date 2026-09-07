---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: voltaiq.com
  spf: true
hosts:
- cert_expires: Nov  1 01:32:00 2026 GMT
  host: www.voltaiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Voltaiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voltaiq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Voltaiq
provider_slug: voltaiq
slug: voltaiq-domain-security
source_filename: voltaiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voltaiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 01:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: voltaiq.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltaiq/refs/heads/main/security/voltaiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Batteries
- Energy Storage
- Manufacturing
- Analytics
- Industrial IoT
- Data Management
- Quality
- Electric Vehicles
- Enterprise Software
---

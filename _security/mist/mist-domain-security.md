---
api_specs:
- filename: mist-openapi-original.json
  format: json
  label: Juniper Mist Cloud API
  slug: juniper-mist-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mist/refs/heads/main/openapi/mist-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:certs@mistsys.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mist.com
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.mist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 07:39:33 2026 GMT
  host: api.gc1.mist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.ac2.mist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mist
provider_slug: mist
slug: mist-domain-security
source_filename: mist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: api.gc1.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 07:39:33 2026 GMT\n  hsts: null\n- host: api.ac2.mist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mist.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:certs@mistsys.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mist/refs/heads/main/security/mist-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Networking
- Wireless
- Wi-Fi
- Cloud Management
- Artificial Intelligence
- Network Automation
- Location Services
- Webhooks
- Juniper
---

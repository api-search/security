---
description: ''
domains:
- caa:
  - 0 issue "buypass.com"
  - 0 issue "certainly.com"
  - 0 issue "d-trust.net"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nordea.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: nordea.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nordea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nordea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nordea
provider_slug: nordea
slug: nordea-domain-security
source_filename: nordea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nordea.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nordea.com\n  dnssec: false\n  caa:\n  - 0 issue \"buypass.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"d-trust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordea/refs/heads/main/security/nordea-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Banking
- Finance
- Nordic
---

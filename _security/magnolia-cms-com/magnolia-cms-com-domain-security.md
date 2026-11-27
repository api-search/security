---
description: ''
domains:
- caa:
  - 128 issuewild "letsencrypt.org"
  - 0 issue "rapidssl.com"
  - 0 issuewild "rapidssl.com"
  - 128 issue "amazontrust.com"
  - 128 issue "globalsign.com"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: magnolia-cms.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: magnolia-cms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Magnolia DXP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magnolia DXP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Magnolia DXP
provider_slug: magnolia-cms-com
slug: magnolia-cms-com-domain-security
source_filename: magnolia-cms-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magnolia-cms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: magnolia-cms.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"letsencrypt.org\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issuewild \"rapidssl.com\"\n  - 128 issue \"amazontrust.com\"\n  - 128 issue \"globalsign.com\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/magnolia-cms-com/security/magnolia-cms-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DXP
- Content Management
- Artificial Intelligence
- Enterprise
---

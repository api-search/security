---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forumsys.com
  spf: true
hosts:
- cert_expires: Apr 14 23:59:59 2027 GMT
  host: forumsys.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Forumsys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forum Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Forum Systems
provider_slug: forumsys
slug: forumsys-domain-security
source_filename: forumsys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forumsys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: forumsys.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/forumsys/security/forumsys-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Management
- Security
- Artificial Intelligence
- Enterprise
- Healthcare
---

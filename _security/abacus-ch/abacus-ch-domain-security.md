---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "swisssign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:hostmaster@abainfra.net"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: abacus.ch
  spf: true
hosts:
- cert_expires: Dec 14 08:35:52 2026 GMT
  host: abacus.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abacus Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abacus (Swiss ERP), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Abacus (Swiss ERP)
provider_slug: abacus-ch
slug: abacus-ch-domain-security
source_filename: abacus-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abacus.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 08:35:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abacus.ch\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"swisssign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:hostmaster@abainfra.net\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/abacus-ch/security/abacus-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- ERP
- Finance
- HR
- Procurement
- Manufacturing
---

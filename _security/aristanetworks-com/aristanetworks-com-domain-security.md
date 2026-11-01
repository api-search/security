---
description: ''
domains:
- caa:
  - 0 iodef "mailto:phishing@arista.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aristanetworks.com
  spf: false
hosts:
- cert_expires: Dec 18 15:12:46 2026 GMT
  host: www.aristanetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aristanetworks Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arista Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Arista Networks
provider_slug: aristanetworks-com
slug: aristanetworks-com-domain-security
source_filename: aristanetworks-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aristanetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 15:12:46 2026 GMT\n  hsts: false\ndomains:\n- domain: aristanetworks.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:phishing@arista.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aristanetworks-com/security/aristanetworks-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Networking
- Cloud
- Enterprise
- OpenAPI
---

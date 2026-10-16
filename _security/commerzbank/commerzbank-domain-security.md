---
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-alerts@commerzbank.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commerzbank.de
  spf: true
hosts:
- cert_expires: Mar 26 10:16:29 2027 GMT
  host: www.commerzbank.de
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commerzbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commerzbank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Commerzbank
provider_slug: commerzbank
slug: commerzbank-domain-security
source_filename: commerzbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commerzbank.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 10:16:29 2027 GMT\n  hsts: null\ndomains:\n- domain: commerzbank.de\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa-alerts@commerzbank.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerzbank/refs/heads/main/security/commerzbank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Banking
- Finance
- OpenBanking
- Germany
---

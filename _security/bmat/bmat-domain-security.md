---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:it@bmat.com"
  - 0 issuewild "amazontrust.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bmat.com
  spf: true
hosts:
- cert_expires: Mar 13 10:30:16 2027 GMT
  host: www.bmat.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bmat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bmat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bmat
provider_slug: bmat
slug: bmat-domain-security
source_filename: bmat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bmat.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 13 10:30:16 2027 GMT\n  hsts: false\ndomains:\n- domain: bmat.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:it@bmat.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmat/refs/heads/main/security/bmat-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Music
- Data
- Analytics
- Rights Management
- Platform
---

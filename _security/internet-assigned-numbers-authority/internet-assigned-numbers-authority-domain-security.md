---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuemail "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:caa-reports@icann.org"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: iana.org
  spf: true
hosts:
- cert_expires: Sep 28 21:37:55 2026 GMT
  host: www.iana.org
  hsts: true
  hsts_max_age: 48211200
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 10:59:55 2026 GMT
  host: data.iana.org
  hsts: true
  hsts_max_age: 48211200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Internet Assigned Numbers Authority Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internet Assigned Numbers Authority, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Internet Assigned Numbers Authority
provider_slug: internet-assigned-numbers-authority
slug: internet-assigned-numbers-authority-domain-security
source_filename: internet-assigned-numbers-authority-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iana.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 48211200\n- host: data.iana.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 10:59:55 2026 GMT\n  hsts: true\n  hsts_max_age: 48211200\ndomains:\n- domain: iana.org\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuemail \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:caa-reports@icann.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet-assigned-numbers-authority/refs/heads/main/security/internet-assigned-numbers-authority-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Domains
- DNS
- IP Addressing
- Media Types
- Protocols
- Standards
- Timezones
---

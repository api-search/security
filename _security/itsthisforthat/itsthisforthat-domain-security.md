---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: itsthisforthat.com
  spf: true
hosts:
- cert_expires: Aug 31 05:28:22 2026 GMT
  host: itsthisforthat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itsthisforthat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ItsThisForThat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ItsThisForThat
provider_slug: itsthisforthat
slug: itsthisforthat-domain-security
source_filename: itsthisforthat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itsthisforthat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:28:22 2026 GMT\n  hsts: false\ndomains:\n- domain: itsthisforthat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itsthisforthat/refs/heads/main/security/itsthisforthat-domain-security.yml
summary_line: TLSv1.3
tags:
- Test Data
- Public APIs
---

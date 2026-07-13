---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thispersondoesnotexist.com
  spf: false
hosts:
- cert_expires: Aug 21 15:50:06 2026 GMT
  host: thispersondoesnotexist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: This Person Does Not Exist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for This Person Does not Exist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: This Person Does not Exist
provider_slug: this-person-does-not-exist
slug: this-person-does-not-exist-domain-security
source_filename: this-person-does-not-exist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thispersondoesnotexist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 15:50:06 2026 GMT\n  hsts: false\ndomains:\n- domain: thispersondoesnotexist.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/this-person-does-not-exist/refs/heads/main/security/this-person-does-not-exist-domain-security.yml
summary_line: TLSv1.3
tags:
- Test Data
- Public APIs
---

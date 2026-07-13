---
description: ''
domains:
- caa:
  - 128 issue "digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226"
  - 128 iodef "mailto:security@netlify.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netlify.app
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: vampire-diaries-api.netlify.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Vampire Diaries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Vampire Diaries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Vampire Diaries
provider_slug: the-vampire-diaries
slug: the-vampire-diaries-domain-security
source_filename: the-vampire-diaries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vampire-diaries-api.netlify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netlify.app\n  dnssec: false\n  caa:\n  - 128 issue \"digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226\"\n  - 128 iodef \"mailto:security@netlify.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-vampire-diaries/refs/heads/main/security/the-vampire-diaries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Public APIs
---

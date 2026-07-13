---
api_specs:
- filename: meteor-ddp.yml
  format: yaml
  label: Meteor
  slug: meteor
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/meteor/refs/heads/main/async-apis/meteor-ddp.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: meteor.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.meteor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:53:09 2026 GMT
  host: docs.meteor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meteor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meteor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Meteor
provider_slug: meteor
slug: meteor-domain-security
source_filename: meteor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meteor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.meteor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:53:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meteor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meteor/refs/heads/main/security/meteor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Full-Stack
- JavaScript
- Mobile Development
- Real-Time
- Web Development
---

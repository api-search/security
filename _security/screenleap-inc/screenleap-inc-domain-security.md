---
api_specs:
- filename: screenleap-inc-screen-sharing-openapi.yml
  format: yaml
  label: Screenleap Screen Sharing API
  slug: screenleap-screen-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenleap-inc/refs/heads/main/openapi/screenleap-inc-screen-sharing-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:support@screenleap.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: screenleap.com
  spf: true
hosts:
- cert_expires: Sep 13 04:12:47 2026 GMT
  host: www.screenleap.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 04:12:47 2026 GMT
  host: api.screenleap.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Screenleap Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Screenleap Inc, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Screenleap Inc
provider_slug: screenleap-inc
slug: screenleap-inc-domain-security
source_filename: screenleap-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.screenleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.screenleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: screenleap.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:support@screenleap.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenleap-inc/refs/heads/main/security/screenleap-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Screen Sharing
- Video Conferencing
- Collaboration
- Real-Time Communication
- WebRTC
- Embedded
- Developer Tools
---

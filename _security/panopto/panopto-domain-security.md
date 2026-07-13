---
api_specs:
- filename: index.html
  format: yaml
  label: Panopto REST API
  slug: panopto-rest-api
  spec_type: OpenAPI
  url: https://demo.hosted.panopto.com/Panopto/api/docs/index.html
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: panopto.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: panopto.com)
  spf: false
hosts:
- cert_expires: Sep  2 14:09:57 2026 GMT
  host: www.panopto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: support.panopto.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: <panoptoserverurl>(i.e. example.hosted.panopto.com)
  https: false
kind: domain-security
layout: security
method: probed
name: Panopto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panopto, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Panopto
provider_slug: panopto
slug: panopto-domain-security
source_filename: panopto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.panopto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 14:09:57 2026 GMT\n  hsts: false\n- host: support.panopto.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: <panoptoserverurl>(i.e. example.hosted.panopto.com)\n  https: false\ndomains:\n- domain: panopto.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: panopto.com)\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/security/panopto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video Management
- Education Technology
- Enterprise Video
- Recording
- Learning Management
- Video Analytics
- Content Management
---

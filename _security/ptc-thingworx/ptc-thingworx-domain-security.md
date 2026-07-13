---
api_specs:
- filename: ptc-thingworx-rest-openapi.yml
  format: yaml
  label: PTC ThingWorx REST API
  slug: thingworx-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-rest-openapi.yml
- filename: ptc-thingworx-websocket-asyncapi.yml
  format: yaml
  label: PTC ThingWorx WebSocket/AlwaysOn API
  slug: thingworx-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/asyncapi/ptc-thingworx-websocket-asyncapi.yml
description: ''
domains:
- caa:
  - 128 issue "quovadisglobal.com"
  - 128 issuewild "digicert.com"
  - 128 issuewild "pki.goog"
  - 128 issuewild "quovadisglobal.com"
  - 128 issuewild "amazon.com"
  - 128 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ptc.com
  spf: true
hosts:
- host: docs.ptc.com
  https: false
- cert_expires: Aug 28 23:59:59 2026 GMT
  host: www.ptc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ptc Thingworx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ptc-thingworx, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ptc-thingworx
provider_slug: ptc-thingworx
slug: ptc-thingworx-domain-security
source_filename: ptc-thingworx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.ptc.com\n  https: false\n- host: www.ptc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ptc.com\n  dnssec: false\n  caa:\n  - 128 issue \"quovadisglobal.com\"\n  - 128 issuewild \"digicert.com\"\n  - 128 issuewild \"pki.goog\"\n  - 128 issuewild \"quovadisglobal.com\"\n  - 128 issuewild \"amazon.com\"\n  - 128 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/security/ptc-thingworx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---

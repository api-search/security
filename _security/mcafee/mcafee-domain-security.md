---
api_specs:
- filename: mcafee-epo-openapi.yml
  format: yaml
  label: McAfee ePO API
  slug: mcafee-epo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-epo-openapi.yml
- filename: mcafee-mvision-openapi.yml
  format: yaml
  label: McAfee MVISION API
  slug: mcafee-mvision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-mvision-openapi.yml
- filename: mcafee-web-gateway-openapi.yml
  format: yaml
  label: McAfee Web Gateway API
  slug: mcafee-web-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-web-gateway-openapi.yml
- filename: mcafee-esm-openapi.yml
  format: yaml
  label: McAfee ESM API
  slug: mcafee-esm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/openapi/mcafee-esm-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trellix.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mcafee.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.trellix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.mvision.mcafee.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mcafee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McAfee (Trellix), probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: McAfee (Trellix)
provider_slug: mcafee
slug: mcafee-domain-security
source_filename: mcafee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trellix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\n- host: api.mvision.mcafee.com\n  https: false\ndomains:\n- domain: trellix.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mcafee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/security/mcafee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Antivirus
- Cybersecurity
- Endpoint Protection
- Security
- Threat Intelligence
---

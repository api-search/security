---
api_specs:
- filename: cradlepoint-netcloud-manager-api-v2-openapi.yml
  format: yaml
  label: Cradlepoint NetCloud Manager API v2
  slug: netcloud-manager-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-netcloud-manager-api-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cradlepoint.com
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cradlepointecm.com
  spf: true
hosts:
- cert_expires: Sep 16 17:48:39 2026 GMT
  host: cradlepoint.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- host: customer.cradlepoint.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Sep  9 05:58:51 2026 GMT
  host: www.cradlepointecm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cradlepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cradlepoint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cradlepoint
provider_slug: cradlepoint
slug: cradlepoint-domain-security
source_filename: cradlepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cradlepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:48:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: customer.cradlepoint.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: www.cradlepointecm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:58:51 2026 GMT\n  hsts: null\ndomains:\n- domain: cradlepoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cradlepointecm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/security/cradlepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wireless WAN
- 5G
- LTE
- Edge
- Branch Networking
- SD-WAN
- SASE
- Routers
- In-Vehicle
- IoT
- Cellular
- Private 5G
- NetCloud
- Ericsson
---

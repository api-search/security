---
api_specs:
- filename: info
  format: yaml
  label: ipbase IP Geolocation API
  slug: ipbase-ip-geolocation-api
  spec_type: OpenAPI
  url: https://ipbase.com/docs/info
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ipbase.com
  spf: true
hosts:
- cert_expires: Aug 17 11:12:33 2026 GMT
  host: ipbase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 11:12:33 2026 GMT
  host: api.ipbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ipbase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ipbase
provider_slug: ipbase
slug: ipbase-domain-security
source_filename: ipbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 11:12:33 2026 GMT\n  hsts: false\n- host: api.ipbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 11:12:33 2026 GMT\n  hsts: null\ndomains:\n- domain: ipbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipbase/refs/heads/main/security/ipbase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IP Geolocation
- IP Address
- Geolocation
- Security
- VPN Detection
- Proxy Detection
- Timezone
- Currency
- ASN
- Threat Intelligence
---

---
api_specs:
- filename: ipinfo-abuse-api-openapi.yml
  format: yaml
  label: IPinfo abuse API
  slug: ipinfo-abuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-abuse-api-openapi.yml
- filename: ipinfo-asn-api-openapi.yml
  format: yaml
  label: IPinfo asn API
  slug: ipinfo-asn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-asn-api-openapi.yml
- filename: ipinfo-carrier-api-openapi.yml
  format: yaml
  label: IPinfo carrier API
  slug: ipinfo-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-carrier-api-openapi.yml
- filename: ipinfo-company-api-openapi.yml
  format: yaml
  label: IPinfo company API
  slug: ipinfo-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-company-api-openapi.yml
- filename: ipinfo-domains-api-openapi.yml
  format: yaml
  label: IPinfo domains API
  slug: ipinfo-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-domains-api-openapi.yml
- filename: ipinfo-general-api-openapi.yml
  format: yaml
  label: IPinfo general API
  slug: ipinfo-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-general-api-openapi.yml
- filename: ipinfo-ipinfo-core-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo core API
  slug: ipinfo-ipinfo-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-core-api-openapi.yml
- filename: ipinfo-ipinfo-lite-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo lite API
  slug: ipinfo-ipinfo-lite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-lite-api-openapi.yml
- filename: ipinfo-ipinfo-max-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo max API
  slug: ipinfo-ipinfo-max-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-max-api-openapi.yml
- filename: ipinfo-ipinfo-plus-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo plus API
  slug: ipinfo-ipinfo-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-plus-api-openapi.yml
- filename: ipinfo-places-api-openapi.yml
  format: yaml
  label: IPinfo places API
  slug: ipinfo-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-places-api-openapi.yml
- filename: ipinfo-privacy-detection-api-openapi.yml
  format: yaml
  label: IPinfo privacy detection API
  slug: ipinfo-privacy-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-privacy-detection-api-openapi.yml
- filename: ipinfo-privacy-detection-extended-api-openapi.yml
  format: yaml
  label: IPinfo privacy detection extended API
  slug: ipinfo-privacy-detection-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-privacy-detection-extended-api-openapi.yml
- filename: ipinfo-ranges-api-openapi.yml
  format: yaml
  label: IPinfo ranges API
  slug: ipinfo-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ranges-api-openapi.yml
- filename: ipinfo-residential-proxy-detection-api-openapi.yml
  format: yaml
  label: IPinfo residential proxy detection API
  slug: ipinfo-residential-proxy-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-residential-proxy-detection-api-openapi.yml
- filename: ipinfo-single-api-openapi.yml
  format: yaml
  label: IPinfo single API
  slug: ipinfo-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-single-api-openapi.yml
- filename: ipinfo-whois-api-openapi.yml
  format: yaml
  label: IPinfo whois API
  slug: ipinfo-whois-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-whois-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ipinfo.io
  spf: true
hosts:
- cert_expires: Sep 15 15:37:33 2026 GMT
  host: ipinfo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:37:33 2026 GMT
  host: api.ipinfo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:37:33 2026 GMT
  host: v6.ipinfo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipinfo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPinfo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IPinfo
provider_slug: ipinfo
slug: ipinfo-domain-security
source_filename: ipinfo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipinfo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:37:33 2026 GMT\n  hsts: false\n- host: api.ipinfo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:37:33 2026 GMT\n  hsts: null\n- host: v6.ipinfo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:37:33 2026 GMT\n  hsts: false\ndomains:\n- domain: ipinfo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/security/ipinfo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IP Intelligence
- IP Geolocation
- ASN
- Privacy Detection
- VPN Detection
- Threat Intelligence
- Network Data
- Mobile Carrier
- WHOIS
- Public APIs
- Development
---

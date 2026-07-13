---
api_specs:
- filename: abuseipdb-apiv2-openapi.yml
  format: yaml
  label: AbuseIPDB APIv2
  slug: apiv2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abuseipdb/refs/heads/main/openapi/abuseipdb-apiv2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: abuseipdb.com
  spf: true
hosts:
- cert_expires: Oct  9 04:12:19 2026 GMT
  host: www.abuseipdb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 04:12:19 2026 GMT
  host: docs.abuseipdb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 04:12:19 2026 GMT
  host: api.abuseipdb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abuseipdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AbuseIPDB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: AbuseIPDB
provider_slug: abuseipdb
slug: abuseipdb-domain-security
source_filename: abuseipdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abuseipdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:12:19 2026 GMT\n  hsts: null\n- host: docs.abuseipdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:12:19 2026 GMT\n  hsts: false\n- host: api.abuseipdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:12:19 2026 GMT\n  hsts: null\ndomains:\n- domain: abuseipdb.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abuseipdb/refs/heads/main/security/abuseipdb-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Anti Malware
- Blacklist
- Cyber Security
- IP Reputation
- Network Security
- Public APIs
- Threat Intelligence
---

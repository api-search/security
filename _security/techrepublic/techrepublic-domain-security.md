---
api_specs:
- filename: techrepublic-wordpress-rest-api-openapi.yml
  format: yaml
  label: TechRepublic WordPress REST API
  slug: wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techrepublic/refs/heads/main/openapi/techrepublic-wordpress-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: techrepublic.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Aug 26 06:34:38 2026 GMT
  host: www.techrepublic.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:43:58 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Techrepublic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TechRepublic, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TechRepublic
provider_slug: techrepublic
slug: techrepublic-domain-security
source_filename: techrepublic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.techrepublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:34:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:43:58 2026 GMT\n  hsts: false\ndomains:\n- domain: techrepublic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techrepublic/refs/heads/main/security/techrepublic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Enterprise IT
- Media
- Technology News
- Content
- Publishing
---

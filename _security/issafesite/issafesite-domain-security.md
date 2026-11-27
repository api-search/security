---
api_specs:
- filename: issafesite-openapi-generated.yml
  format: yaml
  label: IsSafeSite API
  slug: issafesite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/issafesite/openapi/_ae-authored/issafesite-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: issafesite.com
  spf: true
hosts:
- cert_expires: Jan 28 12:35:17 2027 GMT
  host: issafesite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IsSafeSite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IsSafeSite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: IsSafeSite
provider_slug: issafesite
slug: issafesite-domain-security
source_filename: issafesite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: issafesite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 12:35:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: issafesite.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/issafesite/security/issafesite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Websites
- Scanner
- Artificial Intelligence
- Compliance
- Monitoring
---

---
api_specs:
- filename: ipwho-org-openapi-generated.yml
  format: yaml
  label: IPWho.org API
  slug: ipwho-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipwho-org/openapi/_ae-authored/ipwho-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ipwho.org
  spf: false
hosts:
- cert_expires: Dec 20 12:25:32 2026 GMT
  host: www.ipwho.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ipwho Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPWho.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: IPWho.org
provider_slug: ipwho-org
slug: ipwho-org-domain-security
source_filename: ipwho-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ipwho.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 12:25:32 2026 GMT\n  hsts: false\ndomains:\n- domain: ipwho.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ipwho-org/security/ipwho-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- IP Geolocation
- Developer-Friendly
- Free Tier
---

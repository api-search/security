---
api_specs:
- filename: cloudshare-openapi-generated.yml
  format: yaml
  label: Cloudshare API
  slug: cloudshare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/_ae-authored/cloudshare-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudshare.com
  spf: true
hosts:
- cert_expires: Dec 21 19:27:00 2026 GMT
  host: www.cloudshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudshare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudshare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudshare
provider_slug: cloudshare
slug: cloudshare-domain-security
source_filename: cloudshare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 19:27:00 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/security/cloudshare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- VirtualLabs
- Training
- Sandbox
- Enterprise
---

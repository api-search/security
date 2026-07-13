---
api_specs:
- filename: ovh-cloud-openapi-original.yml
  format: yaml
  label: OVH Cloud API
  slug: ovh-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ovh-cloud/refs/heads/main/openapi/ovh-cloud-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ovhcloud.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: us.ovhcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 06:54:41 2026 GMT
  host: api.us.ovhcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ovh Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OVH Cloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OVH Cloud
provider_slug: ovh-cloud
slug: ovh-cloud-domain-security
source_filename: ovh-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.ovhcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.us.ovhcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:54:41 2026 GMT\n  hsts: false\ndomains:\n- domain: ovhcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ovh-cloud/refs/heads/main/security/ovh-cloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- Compute
- Servers
- Hosting
---

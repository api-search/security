---
api_specs:
- filename: asyncapi.yml
  format: yaml
  label: Filestack
  slug: filestack
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/filestack/refs/heads/main/asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: filestack.com
  spf: true
hosts:
- cert_expires: Sep 17 21:33:21 2026 GMT
  host: www.filestack.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Filestack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filestack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Filestack
provider_slug: filestack
slug: filestack-domain-security
source_filename: filestack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.filestack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 21:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: filestack.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filestack/refs/heads/main/security/filestack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage And File Sharing
- Public APIs
---

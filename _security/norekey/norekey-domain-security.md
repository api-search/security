---
api_specs:
- filename: norekey-api-openapi.json
  format: json
  label: NoRekey API API
  slug: norekey-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norekey/openapi/_original/norekey-api-openapi.json
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: norekey.com
  spf: true
hosts:
- cert_expires: Dec  5 20:57:45 2026 GMT
  host: norekey.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Norekey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NoRekey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: NoRekey
provider_slug: norekey
slug: norekey-domain-security
source_filename: norekey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: norekey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 20:57:45 2026 GMT\n  hsts: false\ndomains:\n- domain: norekey.com\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/norekey/security/norekey-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Data Conversion
- Software-as-a-Service
- Banking
---
